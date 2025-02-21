# **Roteiro de Apresentação - DEMO INDIVIDUAL**

## **1. Introdução**

### **Autopresentação**
- Apresente-se brevemente, incluindo uma autodescrição, se necessário.

### **Abertura**
- Explique que escolheu uma tarefa desafiadora para apresentar.  
- Introduza o **OneClick**:  
  > "O OneClick é um produto criado para reduzir o impacto ao cliente durante momentos de crise. Ele automatiza processos que antes eram realizados manualmente, economizando tempo e diminuindo riscos operacionais."

---

## **2. Slide 1 - Contextualização**

- Dê um exemplo prático:  
  > "Imagine que ocorre um problema no Extrato hospedado na AWS e é necessário migrar rapidamente para o ambiente OnPremise. Antes, isso demandava um processo manual e demorado. Agora, com o OneClick, essa troca é feita em segundos, apenas alterando uma chave."  

- Outros processos automatizados pelo OneClick incluem:  
  - **Saldo**  
  - **Login do One Itaú (PF)**  
  - **Pix** (foco da apresentação).  

---

## **3. Slide 2 - A Automação no Pix**

### **Descrição da Automação**
- Permite alterar o IP de comunicação com o Banco Central nas transações Pix.  
- O tráfego pode passar pelo:  
  - **DNS** (load balancer).  
  - **IPs específicos** (66 ou 67).  

- Essa configuração é definida em um arquivo no servidor.

---

## **4. Demonstração Técnica**

### **Abertura do Arquivo .conf**
1. Abra o servidor e exiba o arquivo de configuração.  
2. Explique as linhas de configuração, destacando os conceitos:  
   - **DICT (Diretório de Identificadores de Contas Transacionais)**: Banco de dados que mapeia chaves Pix às contas dos usuários.  
   - **ICOM (Interface de Comunicação)**: Conecta o Itaú ao Banco Central para transações Pix.  
   - **ARQ (Arquitetura de Resiliência)**: Garante a continuidade e segurança do serviço Pix.  

### **Estado Atual**
- Mostre que a linha ativa é do **DNS**, indicando que o tráfego está balanceado entre os IPs 66 e 67.

---

## **5. Explicação do Fluxo do Pix**

1. **Simulação de Transação**:  
   - Imagine que **Vinícius** deve R$50 ao **Rogerinho** e inicia o pagamento via Pix, informando a chave Pix do Rogério.  
   - O sistema consulta o **DICT** pelo IP ativo (**DNS**) e verifica a conta vinculada à chave.  

2. **Processamento da Transação**:  
   - Ocorre comunicação via **ICOM** com o Banco Central e a instituição do Rogério para autenticar a transação.  
   - O Banco Central debita o valor da conta do Vinícius e credita na conta do Rogério, processando tudo em tempo real.  

3. **Notificação Final**:  
   - Ambas as partes são notificadas sobre o sucesso ou falha da operação.  

4. **Relação com o Arquivo .conf**:  
   - Todo o tráfego dessa transação passa pelos IPs definidos no arquivo de configuração.

---

## **6. Demonstração Prática - Simulando uma Crise**

### **Cenário: Problema no IP 66**
1. Acesse o **OneClick** e altere a chave para utilizar apenas o IP 67.  
2. Explique cada passo:  
   - Insira o número do incidente válido.  
   - Realize a alteração e aguarde o processo ser concluído.  

### **Resultado**
- Mostre que:  
  - No arquivo do servidor, a linha do **DNS** está comentada.  
  - O **OneClick** exibe corretamente a alteração.  
  - O tráfego ocorre apenas pelo **IP 67**.

---

## **7. Fechamento**

### **Reconhecimento do Trabalho**
- "Essa automação, que eu desenvolvi no backend do OneClick, foi possível graças à colaboração com Zerati, Rogerinho, Yuri e outras áreas."

### **Desafios Superados**
- "Apesar de desafios como acessos e permissões no servidor, conseguimos entregar a funcionalidade com sucesso."

### **Conclusão**
- Finalize agradecendo e abra para perguntas ou comentários.
