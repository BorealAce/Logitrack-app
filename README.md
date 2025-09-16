# LogiTrack - Sistema de Gerenciamento de Robôs Logísticos

Aplicativo móvel para gerenciamento e monitoramento de robôs logísticos, desenvolvido com React Native e Expo.

## Requisitos

- Node.js (versão 14 ou superior)
- npm ou yarn
- Expo CLI
- Backend Spring Boot rodando em http://localhost:8080

## Instalação

1. Clone o repositório:
```bash
git clone [URL_DO_REPOSITORIO]
cd logitrack-app
```

2. Instale as dependências:
```bash
npm install
# ou
yarn install
```

3. Inicie o aplicativo:
```bash
npm start
# ou
yarn start
```

4. Escaneie o QR code com o aplicativo Expo Go no seu dispositivo móvel ou pressione:
- `a` para abrir no emulador Android
- `i` para abrir no simulador iOS
- `w` para abrir no navegador web

## Funcionalidades

- **Dashboard**: Visualização geral do sistema com contadores e gráficos
- **Gerenciamento de Robôs**: Lista e controle de robôs logísticos
- **Monitoramento de Sensores**: Acompanhamento de leituras e alertas
- **Rastreamento de Entregas**: Acompanhamento de entregas em tempo real

## Estrutura do Projeto

```
src/
├── components/     # Componentes reutilizáveis
├── screens/        # Telas do aplicativo
├── services/       # Serviços de API
├── utils/          # Funções utilitárias
├── context/        # Contextos do React
├── assets/         # Recursos estáticos
├── constants/      # Constantes e temas
└── navigation/     # Configuração de navegação
```

## Tecnologias Utilizadas

- React Native
- Expo
- React Navigation
- React Native Paper
- React Native Chart Kit
- Axios
- AsyncStorage

## Alinhamento
1. Novas telas adicionadas:
- RegisterScreen (Cadastro de usuário)
- UserManagementScreen (Administração de usuários)
- EditUserScreen (Edição de usuário)
- RegisterUserScreen (Cadastro de usuário pelo admin)

2. Funcionalidade de Edição de Usuário
- Implementação da tela EditUserScreen.js para editar dados do usuário, inclusive senha (opcional).
- Novo serviço updateUser em authService.js para atualizar dados do usuário via API.

3. Aprimoramento do ProfileScreen
- ProfileScreen.js agora carrega dados do usuário do AsyncStorage e exibe nome, email, etc.
- Botão de logout com confirmação.

4. Novas funcionalidades
- Cadastro de usuário.
- Edição de usuário.
- Gestão de usuários para administradores.