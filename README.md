# Flutter Utilizando Supabase

> Aplicativo Flutter para armazenamento offline utilizando SQLite, com suporte a internacionalização, gerenciamento de estado via Provider e práticas modernas de desenvolvimento.

---

## 📋 Índice

- [Sobre o Projeto](#sobre-o-projeto)  
- [Funcionalidades](#funcionalidades)  
- [Tecnologias Utilizadas](#tecnologias-utilizadas)  
- [Requisitos](#requisitos)  
- [Instalação e Execução](#instalação-e-execução)  
- [Internacionalização (i18n)](#internacionalização-i18n)  
- [Testes Automatizados](#testes-automatizados)  
- [Integração Contínua (CI/CD)](#integração-contínua-cicd)  
- [Estrutura do Projeto](#estrutura-do-projeto)  
- [Contribuindo](#contribuindo)  
- [Licença](#licença)  

---

## Sobre o Projeto

O **sqlite_offline** é um aplicativo Flutter que demonstra como implementar armazenamento local eficiente usando SQLite. O projeto incorpora boas práticas de desenvolvimento, incluindo:

- Gerenciamento de estado com Provider  
- Internacionalização para múltiplos idiomas (Português e Inglês)  
- Análise estática de código para garantir qualidade  
- Testes unitários e de widget para maior confiabilidade  
- Automação de build e testes via GitHub Actions  

Este projeto é ideal para quem deseja aprender a construir apps Flutter robustos com persistência local e arquitetura organizada.

---

## Funcionalidades

- **Armazenamento Offline:** Salve e recupere dados localmente usando SQLite.  
- **Gerenciamento de Estado:** Atualize a interface de forma reativa com Provider.  
- **Suporte Multilíngue:** Interface disponível em Português e Inglês, com fácil expansão para outros idiomas.  
- **Testes Automatizados:** Cobertura de testes para lógica e interface.  
- **CI/CD:** Pipeline configurado para garantir qualidade contínua.  
- **Ícones Personalizados:** Suporte completo para Android e iOS.  

---

## Tecnologias Utilizadas

- [Flutter](https://flutter.dev/)  
- [SQLite](https://www.sqlite.org/index.html)  
- [Provider](https://pub.dev/packages/provider)  
- [Flutter Localizations](https://docs.flutter.dev/development/accessibility-and-localization/internationalization)  
- [GitHub Actions](https://github.com/features/actions)  
- [Google Fonts](https://pub.dev/packages/google_fonts)  

---

## Requisitos

- Flutter SDK >= 3.5.1  
- Dart SDK >= 3.5.1  
- Dispositivo físico ou emulador configurado para execução  

---

## Instalação e Execução

1. Clone o repositório:  
   ```bash
   git clone https://github.com/seu_usuario/sqlite_offline.git
   cd sqlite_offline
   ```

2. Instale as dependências:  
   ```bash
   flutter pub get
   ```

3. Execute o app em um dispositivo ou emulador:  
   ```bash
   flutter run
   ```

---

## Internacionalização (i18n)

- Arquivos de tradução localizados em `lib/l10n/` (`intl_en.arb`, `intl_pt.arb`).  
- Para adicionar um novo idioma:  
  1. Crie um arquivo `.arb` com as traduções correspondentes.  
  2. Atualize a lista `supportedLocales` em `main.dart`.  
  3. Execute `flutter pub get` e reconstrua o app.  

---

## Testes Automatizados

- Execute todos os testes com:  
  ```bash
  flutter test
  ```

- Os testes cobrem tanto a lógica de negócio quanto a interface, garantindo estabilidade e qualidade do app.

---

## Integração Contínua (CI/CD)

- Workflow configurado com GitHub Actions para:  
  - Instalar dependências  
  - Executar análise estática (`flutter analyze`)  
  - Rodar testes automatizados (`flutter test`)  
  - Gerar build de release (opcional)  

- Arquivo de configuração: `.github/workflows/flutter_ci.yaml`

---

## Estrutura do Projeto

```
lib/
├── l10n/               # Arquivos de localização (.arb)
├── models/             # Modelos e ChangeNotifiers
├── screens/            # Telas principais
├── services/           # Serviços (ex: acesso a banco)
├── utils/              # Funções utilitárias
├── widgets/            # Widgets reutilizáveis
test/                   # Testes unitários e de widget
assets/
  └── images/           # Imagens e ícones
```

---

## Contribuindo

Contribuições são muito bem-vindas! Para colaborar:

1. Faça um fork do projeto  
2. Crie uma branch para sua feature:  
   ```bash
   git checkout -b feature/nome-da-feature
   ```
3. Faça commit das suas alterações:  
   ```bash
   git commit -m "Descrição clara da feature"
   ```
4. Envie para o repositório remoto:  
   ```bash
   git push origin feature/nome-da-feature
   ```
5. Abra um Pull Request explicando suas mudanças.
