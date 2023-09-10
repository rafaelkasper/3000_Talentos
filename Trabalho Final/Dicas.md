Para iniciar vou dar algumas dicas de como organizar o menu principal:

- Hemocentro
 ```js
function menu() {
  var opcao = Number(
    prompt(`
    ===== SISTEMA DE CADASTRO DE DOADORES DE SANGUE =====
    1. Cadastrar doador
    2. Listar doadores
    3. Buscar doador por tipo sanguíneo
    4. Buscar doador por data da última doação
    5. Sair
    Escolha uma opção:`)
  );

  switch (opcao) {
    case 1:
      cadastrarDoador();
      break;
    case 2:
      listarDoadores();
      break;
    case 3:
      buscarTipoSangue();
      break;
    case 4:
      buscarPorData();
      break;
    case 5:
      // Sair
      break;
    default:
      alert("Opção inválida. Tente novamente.");
      menu();
  }
}
```

- Abrigos
  ```js
  function menu() {
  let opcao = Number(
    prompt(`
      ===== SISTEMA DE CADASTRO DE ABRIGOS =====
      1. Cadastrar abrigo
      2. Listar abrigos
      3. Procurar abrigo
      4. Sair
      Escolha uma opção:`)
  );

  switch (opcao) {
    case 1:
      cadastrarAbrigo();
      break;
    case 2:
      listarAbrigos();
      break;
    case 3:
      procurarAbrigo();
      break;
    case 4:
      // Sair
      break;
    default:
      alert("Opção inválida. Tente novamente.");
      menu();
  }
}
```
