# 🍽️ Cozinha Sem Desperdício

> Aplicação pensada em WordPress que promove receitas sustentáveis para evitar o desperdício de alimentos.

---

## 🧾 Visão Geral do Projeto

**Nome do Projeto**: Cozinha Sem Desperdício  
**Objetivo**: Criar um portal de receitas sustentáveis que ensina o reaproveitamento de alimentos e combate ao desperdício, promovendo o consumo consciente e saudável.  
**Plataforma**: WordPress  
**Público-alvo**: Famílias, estudantes, cozinheiros iniciantes e qualquer pessoa interessada em reduzir o desperdício de comida.

---

## ✅ Requisitos do Sistema

### Requisitos Funcionais

- RF01 – Usuário pode buscar receitas por ingredientes disponíveis.
- RF02 – Administrador pode cadastrar receitas com campos personalizados.
- RF03 – Usuário pode favoritar receitas.
- RF04 – Receita pode conter tags como “sobras de arroz”, “casca de banana”, etc.
- RF05 – Comentários e avaliações nas receitas.
- RF06 – Sugestões de substituições de ingredientes.
- RF07 – Exibição de "Dica do Dia".

### Requisitos Não Funcionais

- RNF01 – Interface responsiva.
- RNF02 – URLs amigáveis e otimizadas para SEO.
- RNF03 – Tempo de carregamento inferior a 2 segundos.
- RNF04 – Interface acessível (alto contraste, leitura por leitores de tela).

---

## 🧱 Arquitetura da Aplicação

- **Frontend (View)**: Tema WordPress personalizado e responsivo.
- **Backend (Controller)**: Custom Post Types + campos personalizados com ACF.
- **Model (Dados)**: Banco MySQL com postagens customizadas e taxonomias.

---

## 📦 Estrutura de Dados

### Custom Post Type: `receita`

Campos personalizados:
- Ingredientes
- Modo de preparo
- Tempo de preparo
- Porções
- Dica de reaproveitamento
- Substituições possíveis
- Avaliação média

### Taxonomias:

- Tipo de alimento (frutas, legumes, grãos)
- Situação (sobras, cascas, folhas)
- Dificuldade (fácil, média, avançada)
- Refeição (almoço, lanche, sobremesa)

---

## 🎯 Diagrama de Casos de Uso

[Administrador] --> (Cadastrar Receita)
[Administrador] --> (Cadastrar Dica do Dia)
[Usuário] --> (Buscar Receita por Ingrediente)
[Usuário] --> (Favoritar Receita)
[Usuário] --> (Comentar Receita)
[Usuário] --> (Avaliar Receita)



---

## 🔌 Plugins e Recursos Utilizados

- Advanced Custom Fields (ACF)
- Custom Post Type UI
- WP Recipe Maker
- WP User Favorites
- FacetWP
- Elementor (opcional)

---

## 🗂️ Estrutura do Tema Personalizado

/wp-content/themes/cozinha-sem-desperdicio/
├── functions.php
├── single-receita.php
├── archive-receita.php
├── template-parts/
│ └── receita-card.php
├── assets/
│ ├── css/
│ └── js/

---

## 🧠 Recursos Extras

- Busca por ingredientes digitados
- Página de “Desafio da Semana”
- Dica rotativa do dia
- Sistema de reputação para usuários ativos

---

## 🔗 Modelo ER (Entidade-Relacionamento)

USUÁRIO (id, nome, email)
└── (N) COMENTÁRIO (id, user_id, receita_id, texto)

RECEITA (id, título, descrição, ingredientes, modo_preparo)
└── (N) FAVORITOS (user_id, receita_id)
└── (N) AVALIAÇÃO (user_id, nota)


---

## ⏱️ Cronograma de Desenvolvimento

| Etapa                         | Duração Estimada |
|------------------------------|------------------|
| Planejamento e Wireframe     | 2 dias           |
| Modelagem dos dados          | 2 dias           |
| Customização do tema         | 5 dias           |
| Implementação dos plugins    | 3 dias           |
| Inserção de receitas piloto  | 2 dias           |
| Testes e ajustes             | 3 dias           |
| Documentação final           | 1 dia            |

---

## 🌱 Considerações Finais

O projeto **Cozinha Sem Desperdício** oferece uma solução sustentável e educativa ao transformar o WordPress em uma plataforma funcional para reaproveitamento de alimentos, contribuindo para a redução de desperdício e estimulando uma alimentação mais consciente e criativa.

---


