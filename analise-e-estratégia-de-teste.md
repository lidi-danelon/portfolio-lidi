# Análise e estratégia de teste  

## 1. Visão geral do produto — um parágrafo curto descrevendo o que é o SauceDemo, qual é sua função principal e quem seria o usuário.  
SauceDemo é um site próprio de teste que representa um e-commerce, ele serve para ajudar os QAs a testarem suas habilidades de qualidade. Sendo o usuário real esses QAs, e o usuário fictício pessoas que querem comprar na internet.
  
## 2. Funcionalidades mapeadas — a lista completa que você levantou explorando o site.  
Login, acessar o menu, mudar filtro, visualizar um produto específico, adicionar e remover produtos do carrinho, colocar os dados para compra e checar os dados e finalizar compra.  
Sendo o fluxo principal e único dele do login à finalização da compra.  
  
## 3. Análise de risco e priorização — aqui é o coração do artefato. Para cada funcionalidade, você vai indicar o nível de prioridade (alta, média ou baixa) e justificar o porquê com base no impacto de uma falha.  
**Alta:** Login; adicionar e remover produtos; checkout.  

**Login**  
Uma falha aqui impede todos os usuários de acessar o sistema, tornando o produto completamente inutilizável.  
*Cenários a verificar:* login com credenciais válidas, login com senha incorreta, login com usuário inexistente, campos vazios, usuário bloqueado.  

**Adicionar e remover produtos**  
Sendo um site de compras é a funcionalidade principal  

**Checkout**  
Sem ele o produto não concluí sua função, mesmo que o resto funcione  
*Sem esses 3, o produto não funciona*  

**Média:** Mudar filtro; Visualizar um produto específico - Esses dois adicionam uma experiência mais agradável e fácil para o usuário, mas não são fundamentais.  

**Baixa:** Logout; Reset app state; All items - Os itens disponíveis no menu são mais adicionais, não mudam a experiência do e-commerce em si.
