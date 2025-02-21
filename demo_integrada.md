# Roteiro - Demo Integrada

## 1. Introdução Rápida (1 min)

**Apresentação breve:**
> "Boa tarde pessoal! Eu sou o Alan, dev backend aqui na Millennium."

**Contexto geral do OneClick:**
> "O OneClick é uma ferramenta que automatiza processos críticos para reduzir impactos em momentos de crise, permitindo que ações manuais sejam realizadas em segundos por meio de um clique."

---

## 2. Destaques da Nova Feature e Melhorias Recentes (2 min)

### 2.1. Introdução à Automação do Pix
> "Hoje, vou apresentar a automação que criamos para gerenciar o tráfego de dados nas transações Pix, garantindo resiliência e disponibilidade do serviço."

> "Anteriormente, a operação precisava configurar manualmente arquivos no servidor para mudar o IP de comunicação com o Banco Central, um processo demorado e propenso a erros. Agora, isso é feito com um único clique no OneClick."

### 2.2. O que a feature resolve
> "Ela permite alternar automaticamente entre o DNS (balanceamento de carga) e os IPs específicos (66 ou 67), reduzindo o tempo de resposta em situações críticas e garantindo a continuidade das transações Pix."

### 2.3. Melhorias nos Filtros por Categorias
> "Antes de mostrar a automação, destaco que agora o OneClick tem um filtro por categorias: Negócios e Telecom. Isso organiza as automações por área e facilita a navegação."

**Demonstração rápida dos filtros na interface web.**

---

## 3. Demonstração Prática (5 min)

### 3.1. Cenário de Crise Simulado
> "Vamos simular um cenário em que o IP 66 está instável, e precisamos redirecionar o tráfego para o IP 67."

### 3.2. Passos na Automação do Pix
1. Abra o OneClick na interface web.
2. Mostre como informar o incidente e selecionar a chave para alterar.
3. Execute a mudança clicando no botão correspondente.
4. Exiba o arquivo de configuração atualizado no servidor:  
   > "Aqui está o resultado: o DNS foi comentado, e o IP 67 está ativo."

### 3.3. Impacto do Resultado
> "Isso significa que todas as transações Pix passam agora pelo IP ativo, garantindo a continuidade do serviço até que o ambiente volte à normalidade."

### 3.4. Funcionalidade Adicional: Autocadastro de Automações
> "Como novidade, agora podemos cadastrar automações diretamente pela tela do Automation Owner, sem necessidade de acessar o banco de dados via comandos SQL. Isso dá mais autonomia e agilidade à equipe."

**Demonstre rapidamente o cadastro de uma nova automação.**

---

## 4. Impacto e Relevância (1 min)

**Impacto da Automação no OneClick:**
> "Essa automação reflete o objetivo do OneClick: reduzir o tempo de resposta e aumentar a eficiência operacional, garantindo que o Pix — um serviço de alta criticidade — continue disponível e resiliente mesmo em crises."

**Contribuição do Time:**
> "Gostaria de destacar que essa entrega foi possível graças ao trabalho colaborativo entre o time de Frontend, Backend e os parceiros. O esforço conjunto foi fundamental para superar os desafios técnicos e operacionais."

---

## 5. Encerramento (1 min)

**Reconhecimento e Agradecimentos:**
> "Essa entrega foi possível graças à colaboração entre nosso time e áreas parceiras. O trabalho conjunto foi essencial para superar os desafios técnicos e operacionais."

**Chamado para Perguntas:**
> "Agora abro para perguntas ou comentários sobre essa entrega ou outros pontos do OneClick. Obrigado!"






---

### Dicas para a Apresentação

- **Use visuais simples**: Demonstre filtros, automação e alterações no servidor.
- **Conecte-se ao impacto maior**: Destaque a importância para a operação e o cliente final.
- **Controle o tempo**: Ensaiar a demo garante fluidez e deixa espaço para perguntas.

---
