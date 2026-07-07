# Análise e estratégia de teste  

## 1. Visão geral do produto  
SauceDemo é um site de demonstração, criado para fins de prática, que simula um e-commerce. Ele serve para ajudar os QAs a testarem suas habilidades de qualidade. Sendo o usuário real esses QAs, e o usuário fictício pessoas que querem comprar na internet.
  
## 2. Funcionalidades mapeadas  
Login, acessar o menu, mudar filtro, visualizar um produto específico, adicionar e remover produtos do carrinho, colocar os dados para compra, checar os dados e finalizar compra, logout, reset app state e all items.  
Sendo o fluxo principal e único dele do login à finalização da compra.
  
## 3. Análise de risco e priorização  
**Alta:** Login; adicionar e remover produtos; checkout.  

**Login**  
Uma falha aqui impede todos os usuários de acessar o sistema, tornando o produto completamente inutilizável.  
*Cenários a verificar:* login com credenciais válidas, login com senha incorreta, login com usuário inexistente, campos vazios, usuário bloqueado.  

**Adicionar e remover produtos**  
Quando a adição não funciona interrompe o fluxo de compra antes mesmo de ele começar, impedindo o usuário de concluir qualquer transação. No caso da remoção trava pelo usuário querer remover um item que não quer mais e não conseguir, então ele não vai concluir de qualquer forma.  
*Cenários a verificar:* adição e remoção de itens, quantidade de itens, persistência do carrinho ao navegar entre telas, carrinho vazio indo pro checkout.  

**Checkout**  
O checkout falhar deixa o usuário preso depois de já ter navegado e escolhido os produtos, gerando frustração e sensação de tempo perdido.  
*Cenários a verificar:* campos obrigatórios vazios, botão de voltar no meio do fluxo, dados sendo exibidos corretamente na tela de revisão.  

**Média:** Mudar filtro e Visualizar um produto específico - Adicionam uma experiência mais agradável e fácil para o usuário, mas não são fundamentais.  
Logout - O Logout falhar é um problema de segurança — o usuário não consegue encerrar a sessão.  

**Baixa:** Reset app state e All items - Para o usuário fictício, são itens mais adicionais, não mudam a experiência do e-commerce em si. Mas para o usuário real tem mais relevância, ajudando nos testes.

---
  
# Níveis de teste por funcionalidade
