# fastpdfmerge

**Fast PDF Merge Educacional** — Aplicação web moderna, segura e minimalista para mesclagem e organização de propostas e relatórios de recuperação paralela em PDF diretamente no navegador, sem envio para servidores externos.

- **Repositório**: [`profedmarsantos/fastpdfmerge`](https://github.com/profedmarsantos/fastpdfmerge)
- **Aplicação online (GitHub Pages)**: [https://profedmarsantos.github.io/fastpdfmerge/](https://profedmarsantos.github.io/fastpdfmerge/)

---

## 🚀 Funcionalidades

- **100% Processado no Navegador**: Os arquivos PDF e dados acadêmicos nunca saem do dispositivo do usuário (privacidade e segurança total, com escolha entre armazenamento local ou temporário).
- **Cadastros Acadêmicos e Importação do SUAP**:
  - Cadastro de disciplinas de cursos Integrados (bimestral) e Concomitantes/Subsequentes (modular), com suporte a 1 ou 2 professores por disciplina.
  - Importação rápida de diários a partir de arquivo `.mhtml` exportado do SUAP.
- **Mesclagem de Módulos e Bimestres**:
  - Organização em abas separadas (**CADASTROS**, **MÓDULOS**, **BIMESTRES**) com isolamento de contexto por modalidade.
  - Validação de pares completos (**Proposta + Relatório**) e geração automática do formulário oficial **Controle de Recuperação Paralela** (com logotipo do IFSP) para os períodos sem recuperação.
- **Padrão Oficial de Nomenclatura Escolar**:
  - Formato automático de acordo com o ano letivo, código e nome do componente curricular (com opção de personalização).
- **Deploy Automático no GitHub Pages**: Configurado via GitHub Actions em `.github/workflows/deploy.yml`.

---

## 🛠️ Publicando atualizações no GitHub (`fastpdfmerge`)

Para enviar uma atualização de versão para o repositório [`profedmarsantos/fastpdfmerge`](https://github.com/profedmarsantos/fastpdfmerge):

```bash
# Caso o remote local ainda aponte para outro nome, atualize para:
git remote set-url origin https://github.com/profedmarsantos/fastpdfmerge.git

# 1. Adicione os arquivos alterados
git add .

# 2. Crie o commit com a mensagem da versão
git commit -m "chore: release nova versão"

# 3. (Opcional) Crie uma tag de versão
git tag v1.0.1

# 4. Envie as alterações para o GitHub
git push origin main --tags
```

---

## 🌐 Deploy Automático no GitHub Pages

O workflow `.github/workflows/deploy.yml` compila e publica o site automaticamente a cada `git push` na branch `main` (ou `master`) e em tags de versão `v*`.

Configuração no GitHub:
1. Acesse o repositório: [https://github.com/profedmarsantos/fastpdfmerge](https://github.com/profedmarsantos/fastpdfmerge)
2. Acesse **Settings** > **Pages**.
3. Em **Build and deployment** / **Source**, mantenha selecionado **GitHub Actions**.
4. A aplicação fica disponível em:
   **[https://profedmarsantos.github.io/fastpdfmerge/](https://profedmarsantos.github.io/fastpdfmerge/)**

---

## 💻 Desenvolvimento Local

```bash
# Instalar dependências
npm install

# Iniciar servidor de desenvolvimento
npm run dev

# Verificar tipagem TypeScript
npm run lint

# Compilar para produção
npm run build
```
