# Lista de tarefas com VueJS

Aplicativo simples de lista de tarefas feito com VueJS.

A intenção é ter várias formas de guardar os dados, como:

- no armazenamento local do navegador, como já está;
- numa API em PHP com banco MySQL. Já pronto;
- num serviço em Node.JS com banco gerenciado na nuvem — também pronto. Se quiser, dá para converter o código para rodar em função serverless com um framework de deploy, porque o estado não fica em sessão, só no banco externo;
- numa API em Rails usando, por escolha minha, um banco embutido de arquivo: ainda não pronto.

Essas coisas ficam para o futuro.

Há uma gravação da versão atual em uso.

E outra gravação narrada em inglês.


# Outras partes

A versão de API em PHP tem repositório próprio.

A versão de API em Node.JS também.

Dependendo da estratégia escolhida, você vai precisar da parte correspondente.

As estratégias em Node.JS e em PHP esperam o servidor respondendo na porta 8000. Vale olhar o console em busca de erros eventuais.


# Executando

Depende da estratégia. Para a estratégia em PHP, instale a aplicação de servidor indicada acima e rode, na raiz dela:

```
composer install
```

Na versão PHP também é preciso resolver a questão do banco, ajustando o arquivo de configuração.

Com um banco disponível, aplique as migrações:

```
php artisan migrate
```

E suba o servidor web:

```
php artisan serve
```

A parte cliente, que é o conteúdo deste repositório, pode ser servida pelo servidor embutido da linguagem.

Ou você pode simplesmente abrir o arquivo de entrada no navegador.

Se a ideia for usar o armazenamento local do navegador, basta rodar o cliente como descrito acima.

Já a estratégia em Node.JS exige clonar a aplicação servidora indicada acima, em outra pasta, e rodar a instalação de dependências e o serviço.

E claro (kkk), com o cliente deste repositório aberto no navegador.

# Comentários

Para ver o uso das diferentes estratégias de gravação — o mesmo cliente só muda o endereço para onde aponta — vale assistir à demonstração em inglês.


# Ajustes

Assistindo à demonstração em português notei um erro de digitação numa palavra da interface e já corrigi no código.

### Note

Testado na maquina do autor; outro ambiente pode pedir ajuste.