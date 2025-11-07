# Projeto Conta Bancária - Generation Bootcamp Fullstack
---

## 📝 Descrição
Este projeto faz parte do bootcamp Fullstack da Generation Brasil em parceria com o Instituto Caldeira e Instituto Helda Gerdau. O projeto implementa um sistema de conta bancária em TypeScript, demonstrando conceitos de programação orientada a objetos.

## 🚀 Tecnologias Utilizadas
- TypeScript
- Node.js
- readline-sync (para interação no terminal)

## 🧩 Estrutura do Projeto
```
src/
├── model/
│   └── Conta.ts     # Classe principal que implementa a conta bancária
└── util/
    └── Colors.ts    # Utilitário para colorização do terminal
```

### Funcionalidades da Conta
- Criação de conta com número, agência, tipo, titular e saldo
- Operações de saque e depósito
- Visualização dos dados da conta
- Suporte para diferentes tipos de conta (Corrente e Poupança)

## 🛠️ Como Executar o Projeto

1. Clone o repositório:
```bash
git clone https://github.com/andreyrsy/conta-bancaria-bootcamp.git
```

2. Instale as dependências necessárias:
```bash
# Inicialize o projeto Node
npm init -y

# Instale o TypeScript globalmente
npm install -g typescript

# Instale o ts-node globalmente para execução simplificada
npm install -g ts-node

# Inicialize a configuração do TypeScript
tsc --init

# Instale o readline-sync e suas definições de tipos
npm install readline-sync
npm install @types/node
npm install --save-dev @types/readline-sync
```

3. Configure o TypeScript:
Abra o arquivo `tsconfig.json` e faça as seguintes alterações:

```json
{
    // Altere esta configuração para false para permitir imports/exports entre arquivos
    "verbatimModuleSyntax": false,
    
    // Adicione "node" em types para resolver erros com process.exit()
    "types": ["node"]
  }
```

> **Nota sobre configurações:**
> - `"verbatimModuleSyntax": false` - Esta configuração é necessária para permitir a importação/exportação entre arquivos TypeScript usando a sintaxe ES modules. Quando definida como `true`, o TypeScript exige uma sintaxe de módulo mais estrita.
> - `"types": ["node"]` - Esta configuração é necessária para resolver erros relacionados a funcionalidades do Node.js como `process.exit()`. Ela adiciona as definições de tipos do Node.js ao projeto.

4. Execute o projeto:
```bash
ts-node Menu.ts
```

## 🎓 Sobre o Bootcamp Generation
Este projeto é parte de uma jornada de aprendizado no bootcamp Fullstack da Generation Brasil.

### Pastas do Bootcamp Fullstack
- [Projeto JavaScript](https://github.com/andreyrsy/javascript-generation)
- [Projeto TypeScript](https://github.com/andreyrsy/typescript-generation)
- [Projeto Conta Bancária](https://github.com/andreyrsy/conta-bancaria-bootcamp) (Este repositório)

## 📬 Contato
- [GitHub](https://github.com/andreyrsy)

---
⭐ Desenvolvido como parte do programa de Desenvolvimento Fullstack JavaScript da Generation Brasil.