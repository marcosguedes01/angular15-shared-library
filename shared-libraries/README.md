# Criando uma nova biblioteca

É possível criar uma biblioteca apenas dentro de um workspace.
Caso o workspace já este criado, desconsidere o comando abaixo:
```bash
ng new my-workspace --no-create-application
```

Para criar uma nova biblioteca, acesse o workspace criado e utilize o comando `ng generate`, conforme o exemplo abaixo:
```bash
cd my-workspace
ng generate library my-lib
```

# Build da biblioteca
Utilize o comando abaixo para fazer build da biblioteca criada:
```bash
ng build my-lib
```

Para execução dos testes e análise de qualidade, utilize:
```bash
ng test my-lib
ng lint my-lib
```

# Gerando o pacote da biblioteca
```bash
cd dist/my-lib
npm link
npm pack
```

# Instalando uma library em um projeto:
```bash
npm install ../my-lib
```