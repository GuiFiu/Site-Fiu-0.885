<div align="center">

<img src="assets/logo.png" alt="Logo FIU Capoeira" width="130" />

# FIU Capoeira — Sistema de Gestão

**Família Irmãos Unidos · Mestre Sidney**

Painel web para acompanhar presenças, evolução de cordas, mensalidades e a comunicação com os alunos.

`HTML` · `CSS` · `JavaScript` · sem instalação · funciona offline

</div>

---

## Sobre

O sistema nasceu de uma necessidade simples da academia: **parar de controlar presença, cordas e mensalidades em cadernos e planilhas soltas**.

São duas páginas — uma tela de **entrada** e o **painel de gestão** — que rodam direto no navegador. Cada aluno tem seu histórico completo (presenças, frequência, corda atual, tempo de corda, pagamentos e conversas), e o professor ou mestre enxerga tudo em um só lugar.

> **Status:** protótipo funcional de front-end. Os dados ficam no próprio navegador (`localStorage`), o que permite demonstrar o sistema inteiro sem servidor. A próxima etapa é conectar um banco de dados.

---

## Como abrir

Não precisa instalar nada.

1. Baixe ou clone o repositório.
2. Abra o arquivo **`index.html`** no navegador.

Pronto. A tela de entrada abre o painel depois do login.

<details>
<summary>Prefere rodar com um servidor local?</summary>

<br>

```bash
# Python (já vem instalado no macOS e Linux)
python3 -m http.server 8000

# ou Node.js
npx serve .
```

Depois acesse `http://localhost:8000`.
</details>

---

## Contas de demonstração

Na tela de entrada, clique em um dos perfis em **"Acesso rápido"** — usuário e senha são preenchidos automaticamente.

| Perfil | Usuário | Senha | O que enxerga |
|---|---|---|---|
| **Aluno** | `aluno` | `aluno123` | Suas aulas, sua corda e o chat com a academia |
| **Professor** | `professor` | `prof123` | Presenças, alunos, pagamentos e grade |
| **Contra Mestre** | `contramestre` | `contramestre123` | Mesmo acesso do professor |
| **Mestre** | `mestre` | `mestre123` | Acesso completo |

### Painel sem dados?

Ao abrir o painel pela primeira vez, use o botão **✨ Carregar demonstração** (no topo, ao lado do tema). Ele cria 12 alunos, uma grade semanal completa, cerca de dois meses de presenças, mensalidades, conversas e notificações — o suficiente para apresentar o sistema "vivo". Para limpar tudo, o mesmo botão vira **↺ Limpar demonstração**.

---

## O que tem dentro

| Página | Serve para |
|---|---|
| **Presença** | Aulas do dia, calendário mensal do aluno, marcação de presença/falta, histórico das últimas aulas e resumo semanal |
| **Alunos** | Cartões com corda atual, tempo de corda, plano, frequência e situação de pagamento — além de promover, registrar pagamento e remover |
| **Mensagens** | Conversa direta entre academia e aluno, com comprovantes de pagamento enviados automaticamente e aviso de inadimplência |
| **Pagamentos** | Mensalidades em dia / pendentes / atrasadas, receita do mês, valores por plano e histórico dos últimos pagamentos |
| **Permissões** | Tags de acesso geradas a partir do pagamento e da graduação |
| **Grade** | Editor semanal visual (clique na célula para criar a aula) e chamada em massa por turma |
| **Cordas** | As 17 graduações da Família Irmãos Unidos, com significado, cores e tempo mínimo em cada uma |

**Extras que já funcionam:** tema claro/escuro, notificações (com aviso automático de mensalidade atrasada), layout responsivo com menu lateral retrátil, filtros e busca.

---

## Sistema de cordas

A graduação segue o documento da Família Irmãos Unidos — do **Crua (Universo)** ao **Branca (Luz)**, passando por 17 cordas e todos os níveis intermediários (Instrutor, Professor, Contra Mestre e Mestre).

Cada corda tem cor, significado e tempo mínimo de permanência. O sistema calcula sozinho quanto tempo falta para o aluno estar apto a ser promovido.

---

## Estrutura do projeto

```
.
├── index.html          # tela de entrada (login e cadastro)
├── painel.html         # painel de gestão
├── assets/
│   └── logo.png        # logo FIU
└── README.md
```

---

## Detalhes técnicos

- **Sem dependências.** Só HTML, CSS e JavaScript puro — nenhum framework, nenhum build.
- **Dados locais.** O painel salva o estado em `localStorage` (`fiu4`); a sessão fica em `sessionStorage` (`fiu_session`); contas criadas pelo cadastro ficam em `fiu_users`.
- **Temas.** Claro e escuro, com a escolha salva entre visitas.
- **Responsivo.** Funciona em celular e tablet; em telas pequenas o menu lateral vira gaveta.
- **Cuidado com datas.** As datas são montadas com componentes locais, para não "pular" de dia por causa do fuso horário (UTC−3).

---

## Próximos passos

- [ ] Conectar a um backend (Supabase, Firebase ou API própria) para dados compartilhados entre dispositivos
- [ ] Login com senha criptografada no servidor
- [ ] Relatórios em PDF (frequência e inadimplência)
- [ ] Envio real de mensagens (WhatsApp ou e-mail)
- [ ] Área de vídeos e treinos para os alunos

---

<div align="center">

**Família Irmãos Unidos · Capoeira**

*"A arte, a luta, a família."*

</div>
