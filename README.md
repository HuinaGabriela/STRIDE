# STRIDE

## 📌 Descrição

Este projeto consiste em uma API inteligente que realiza modelagem automatizada de ameaças STRIDE a partir de:

📸 Imagens de arquitetura (ex: .drawio.png)

🧾 Informações técnicas da aplicação

Com foco em um sistema de reconhecimento facial com FaceNet e KNN, a API utiliza modelos de linguagem (LLMs) para gerar automaticamente cenários de ameaças realistas e sugestões para melhorar a segurança da aplicação.

💡 Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de:

Automatizar a geração de modelos de ameaças para aplicações sensíveis

Reduzir o tempo gasto em análises manuais de segurança

Aplicar IA generativa multimodal para interpretar imagens e textos técnicos

Avaliar riscos de uma aplicação de reconhecimento facial

Coleta dados biométricos (alta sensibilidade)

Usa autenticação por login

Está exposta via internet (Google Colab, APIs, etc.)

🔎 O que o Agente Analisa

Imagem da arquitetura (.png)

Descrição da aplicação

Tipos de autenticação

Exposição à internet

Uso de dados sensíveis

Com base nisso, a IA gera um relatório em JSON contendo:

Lista de ameaças STRIDE detalhadas (Spoofing, Tampering, etc.)

Sugestões para melhorar a análise em iterações futuras.

Ameaças geradas (exemplo simplificado):

```
{
  "threat_model": [
    {
      "Threat Type": "Information Disclosure",
      "Scenario": "Dados faciais armazenados sem criptografia forte podem ser extraídos por acesso não autorizado ao banco",
      "Potential Impact": "Exposição de dados biométricos dos usuários"
    },
    {
      "Threat Type": "Spoofing",
      "Scenario": "Login baseado apenas em ID pode ser falsificado via engenharia social ou interceptação de requisições",
      "Potential Impact": "Acesso não autorizado à aplicação"
    }
  ],
  "improvement_suggestions": [
    "Descrever como as imagens faciais são protegidas durante o upload e armazenamento",
    "Explicar o fluxo de autenticação detalhado entre componentes"
  ]
}
```


  


