# Classe CreateDir

Esta classe Java, denominada CreateDir, oferece funcionalidades para verificar a existência de um diretório e, se não existir, criá-lo. Foi desenvolvida para simplificar a gestão de diretórios em aplicações Java.

## Método

### `checkAndCreateFolder`

- **Descrição:** Este método verifica a existência de um diretório em um determinado caminho e, se não existir, cria-o.

- **Parâmetros:**
  - `diretory`: O diretório pai onde o diretório será verificado/criado.
  - `folderName`: O nome do diretório que será verificado/criado.

- **Retorna:** `true` se o diretório já existir ou for criado com sucesso, `false` se houver algum erro durante o processo.

- **Exemplo de Uso:**
  ```java
  String diretory = "caminho/do/pai";
  String folderName = "nomeDoDiretorio";
  
  if (CreateDir.checkAndCreateFolder(diretory, folderName)) {
      System.out.println("Diretório verificado/criado com sucesso!");
  } else {
      System.out.println("Erro ao verificar/criar o diretório. Verifique o caminho.");
  }
  ```

## Mensagens de Saída

O método `checkAndCreateFolder` fornece mensagens informativas para cada passo do processo. Aqui estão as mensagens possíveis:

- "Verificando existência da pasta %s no diretório %s..." - Indica que o método está verificando a existência do diretório.
- "Pasta existente" - Indica que o diretório já existe.
- "Pasta %s criada com sucesso" - Indica que o diretório foi criado com sucesso.
- "Erro ao criar pasta. Verifique o diretório" - Indica que ocorreu um erro ao tentar criar o diretório.
- "Verificação concluída" - Indica que o processo de verificação/criação do diretório foi concluído.

Este código é útil para cenários em que é necessário garantir que um determinado diretório esteja disponível antes de prosseguir com outras operações, como criação de arquivos ou manipulação de dados.
