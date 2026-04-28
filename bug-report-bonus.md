## O que aconteceu
Eu estava em um totem em um fastfood, e uma vez fui fazer um pedido e resolvi colocar o CPF por lá quando apareceu na tela pra por. Alguns messes depois, ao tentar criar uma conta no aplicativo deles, teve um problema. Quando tentava criar uma conta do zero o app dizia "Já temos um cadastro nesse CPF", e o CPF para o cadrastro é obrigatório. Mas para realizar o login é necessário preencher o e-mail, que eu não tenho cadastrado justamente por não ter criado minha conta.  
Ou seja, por conta de uma falha na integração entre os dois sistemas eu não consegui criar a conta, e se a falha não for resolvida, nunca. O que seria um bug médio-grave, porque apesar que não ser fundamental para o local vender e funcionar, o objetivo do aplicativo é criar um vínculo mais forte com o cliente, - lá tem descontos exclusivos, facilita com várias formas de pedir a comida - e nesse caso foi perdido.

## Agora transformando isso em um bug report:  

**Título:** *Não é possível criar conta no app por conta de cadastro anterior do CPF feito no totem de autoatendimento* ou *Falha de integração entre totem e app impede o cadastro* (vou decidir a melhor opção de título)

**Ambiente:** Totem de autoatendimento (loja física) e aplicativo (IOS).  

**Passos:**  
1. Ir a uma loja com totem de autoatendimento;
2. Iniciar um pedido;
3. Quando aparecer a opção de colocar o CPF, colocar;
4. Terminar o pedido;
5. Acessar o app;
6. Clicar em "Pedir pelo delivery";
7. Clicar em "É novo aqui? Faça seu cadastro";
8. Colocar um nome;
9. Colocar o CPF usado anteriormente no totem.  

**Resultado esperado:** Avisar que o cadastro já existe, e abrir uma área em que é possível colocar um e-mail e uma senha associados a esse CPF para realizar o cadastro completo.  

**Resultado obtido:** Avisar que o cadastro já existe e para tentar a recuperação de senha, mas como eles usam e-mail para o login não é possível entrar com o CPF.  

**Prioridade:** Média  

**Severidade:** Média-grave  

**Registro:**
