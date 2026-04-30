# avFormadoraII

Aplicativo móvel desenvolvido com **Ionic**, **Angular** e **Capacitor** para Android.

## 📋 Sobre o Projeto

**avFormadoraII** é um aplicativo mobile que oferece funcionalidades de gerenciamento de perfil com suporte a temas personalizados. O app é construído com as tecnologias mais modernas do ecossistema Angular.

### Tecnologias Utilizadas

- **Angular 20** - Framework frontend
- **Ionic 8** - Framework UI para mobile
- **Capacitor 8** - Camada para acesso a APIs nativas do Android
- **TypeScript** - Linguagem de programação
- **RxJS** - Programação reativa
- **SCSS** - Pré-processador CSS

## 🚀 Como Começar

### Pré-requisitos

- **Node.js** (versão 18+)
- **npm** (versão 9+) ou **yarn**
- **Java Development Kit (JDK)** (para builds Android)
- **Android SDK** (para desenvolvimento Android)

### Instalação

1. **Clone o repositório:**
   ```bash
   git clone <url-do-repositorio>
   cd mobile-perfil-rgb-main
   ```

2. **Instale as dependências:**
   ```bash
   npm install
   ```

### Desenvolvimento

#### Executar no Navegador (Development Mode)

```bash
npm start
```

O app estará disponível em `http://localhost:4200`

#### Build para Produção

```bash
npm run build
```

Os arquivos compilados serão gerados na pasta `www/`

#### Observar Mudanças (Watch Mode)

```bash
npm run watch
```

Recompila automaticamente quando há alterações nos arquivos de origem.

### Testes

#### Executar Testes Unitários

```bash
npm test
```

#### Linting

```bash
npm run lint
```

## 📱 Build Android

### Adicionar a Plataforma Android

Se ainda não tiver adicionado:

```bash
npx cap add android
```

### Compilar para Android

1. **Sincronize os arquivos do projeto:**
   ```bash
   npx cap sync
   ```

2. **Abra no Android Studio:**
   ```bash
   npx cap open android
   ```

3. **Build via terminal:**
   ```bash
   cd android
   ./gradlew build
   ```

## 📁 Estrutura do Projeto

```
.
├── src/
│   ├── app/
│   │   ├── home/              # Componente Home
│   │   ├── mudar-cor/         # Componente de Mudança de Cores
│   │   ├── app.component.*    # Componente principal
│   │   └── app.routes.ts      # Rotas da aplicação
│   ├── assets/                # Recursos estáticos
│   ├── environments/          # Configurações de ambiente
│   ├── theme/                 # Temas e estilos globais
│   ├── index.html             # Template HTML
│   ├── main.ts                # Ponto de entrada da aplicação
│   └── global.scss            # Estilos globais
├── android/                   # Código nativo Android (Gradle)
├── www/                       # Build compilado
├── angular.json               # Configuração Angular CLI
├── capacitor.config.ts        # Configuração Capacitor
├── ionic.config.json          # Configuração Ionic
└── package.json               # Dependências e scripts
```

## 🔧 Scripts Disponíveis

| Comando | Descrição |
|---------|-----------|
| `npm start` | Inicia o servidor de desenvolvimento |
| `npm run build` | Faz build para produção |
| `npm run watch` | Observa mudanças e recompila automaticamente |
| `npm test` | Executa testes unitários |
| `npm run lint` | Verifica qualidade do código |

## 🎨 Funcionalidades

- **Gerenciamento de Perfil** - Edição de dados do usuário
- **Mudança de Cores/Temas** - Personalize a aparência do app
- **Interface Responsiva** - Otimizada para dispositivos móveis
- **Integração com APIs Nativas** - Acesso a funcionalidades do Android via Capacitor

## 📦 Dependências Principais

- `@angular/*` - Framework Angular
- `@ionic/angular` - Componentes Ionic
- `@capacitor/*` - Acesso a APIs nativas do dispositivo
- `ionicons` - Biblioteca de ícones
- `rxjs` - Programação reativa
- `zone.js` - Zone.js para Angular

## 🔐 Build e Deploy

### Gerar APK

```bash
cd android
./gradlew assembleDebug    # Debug APK
./gradlew assembleRelease  # Release APK
```

Os arquivos estarão em `android/app/build/outputs/apk/`

## 📝 Contribuindo

1. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
2. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`)
3. Push para a branch (`git push origin feature/MinhaFeature`)
4. Abra um Pull Request

## Autor

**Lucas da Silva de Moura**  
Estudante de Análise e Desenvolvimento de Sistemas

---

**Última atualização:** 29 de abril de 2026
