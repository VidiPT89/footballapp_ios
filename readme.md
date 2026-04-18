# Football App — iOS

Aplicação iOS para acompanhar a Premier League inglesa. Permite consultar as equipas, ver a tabela classificativa e guardar equipas favoritas com notas e avaliações pessoais.

Desenvolvida como projeto de curso na CESAE Digital, em SwiftUI com arquitetura MVVM.

---

## Funcionalidades

- Listagem de todas as equipas da Premier League
- Detalhe de cada equipa (emblema, estádio, ano de fundação, cores e website oficial)
- Tabela classificativa com zonas coloridas (Champions League, Europa League e descida)
- Gestão de favoritas: adicionar, remover, reordenar
- Notas e avaliação pessoal (1 a 5 estrelas) por equipa favorita
- Persistência local das favoritas com SwiftData

---

## Fundação Técnica

| Componente | Tecnologia |
|---|---|
| Linguagem | Swift 5.9 |
| UI Framework | SwiftUI |
| Arquitetura | MVVM com `@Observable` |
| Persistência local | SwiftData |
| API | football-data.org v4 |
| Imagens assíncronas | `AsyncImage` |
| Navegação | `NavigationStack` + `TabView` |

---

## Ecrãs Disponíveis

| Ecrã | Descrição |
|---|---|
| Equipas | Lista de equipas com toggle de favorita |
| Detalhe de Equipa | Informação completa + link para o website oficial |
| Classificação | Tabela com posições e zonas coloridas |
| Favoritas | Lista de equipas guardadas, ordenadas por data |
| Detalhe de Favorita | Informação da equipa + nota e avaliação pessoal |
| Editar Favorita | Formulário para atualizar avaliação e nota |

---

## Requisitos

- Xcode 15 ou superior
- iOS 17 ou superior
- Chave de API válida da [football-data.org](https://www.football-data.org/)

---

## Notas do Programador

- O token da API está hardcoded no `APIHandler.swift` — em produção deveria ser gerido de forma segura (ex.: `.xcconfig` ou Keychain)
- A aplicação está limitada à Premier League (código `PL`); a API suporta outras competições
- Os nomes de variáveis e vistas estão em português, seguindo a convenção do projeto de curso
- Primeiro projeto iOS com SwiftUI e SwiftData

---

## Contexto Académico

Projeto desenvolvido no âmbito do curso de programação na **CESAE Digital**, como exercício de introdução ao desenvolvimento iOS nativo com SwiftUI.
