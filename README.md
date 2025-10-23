# 🧠 Guia Completo de Git e Fork

Este documento explica, passo a passo, como realizar as operações básicas de **Git**, **Fork**, **Clone**, **Commit**, **Push** e **Pull Request**, com base nas etapas mostradas nas imagens da atividade.

---

## 🪄 O Que é o Git?

O **Git** é um sistema de controle de versão distribuído. Ele permite que várias pessoas trabalhem em um mesmo projeto sem sobrescrever o trabalho umas das outras. Cada desenvolvedor tem uma cópia completa do repositório.

### 🔹 Principais Conceitos:

* **Repositório (repo)**: local onde o projeto e seu histórico de alterações são armazenados.
* **Commit**: registro de uma alteração feita no código.
* **Branch**: uma linha de desenvolvimento separada.
* **Merge**: união de mudanças de diferentes branches.
* **Fork**: cópia de um repositório (geralmente usada para contribuir com projetos de outras pessoas).
  
<img width="531" height="231" alt="{A8F10EBE-98F1-4813-954E-23FE455A6BCB}" src="https://github.com/user-attachments/assets/c88d5468-353d-458c-8b3c-b9acb9410907" />


<img width="711" height="354" alt="{B3DE3D1A-2B52-4923-BAE8-E53B66CE03ED}" src="https://github.com/user-attachments/assets/0f96eed7-78e1-46bd-b32d-a7788332bb32" />



---

## 🍴 O Que é um Fork?

O **fork** cria uma cópia completa de um repositório público na sua conta GitHub. Assim, você pode modificar o projeto sem alterar o original.

### 🔹 Quando usar o fork?

* Quando você quer **contribuir com um projeto público**.
* Quando deseja **personalizar** um projeto existente.
* Quando quer **testar mudanças** sem afetar o código original.

### 🔹 Como fazer um fork:

1. Vá até o repositório desejado no **GitHub**.
2. Clique no botão **“Fork”** no canto superior direito.
3. Escolha o destino (sua conta pessoal ou uma organização).
4. Aguarde a criação da cópia do repositório na sua conta.

Exemplo visual (baseado na imagem):

<img width="684" height="309" alt="{85709C5E-30D5-41E8-935B-825C9EA946F2}" src="https://github.com/user-attachments/assets/c4b2481c-f451-4eb9-99bf-ee1c36d5c352" />



```bash
# Depois de fazer o fork, o repositório será copiado para:
https://github.com/seu-usuario/nome-do-repositorio
```


---

## 🧭 Clonando o Repositório Forkado

<img width="1919" height="930" alt="{E321B08F-5567-476A-AECC-B495BFB9ACE4}" src="https://github.com/user-attachments/assets/5bbdb448-19df-4963-813b-529f3a78044f" />

Após fazer o fork, você precisa **clonar** o repositório para seu computador.


### 🔹 Passos para clonar:

1. No seu repositório forkado, clique em **Code**.
2. Copie a URL HTTPS (ou SSH, se configurado).
3. No terminal, digite:

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
```



4. Acesse a pasta do projeto:

```bash
cd nome-do-repositorio
```

Agora você tem uma cópia local do projeto.

---

## ⚙️ Fazendo Alterações e Commits

1. Faça as alterações necessárias nos arquivos do projeto.
2. Verifique o status dos arquivos modificados:

```bash
git status
```

3. Adicione os arquivos alterados à área de stage:

```bash
git add .
```

4. Faça o commit das mudanças:

```bash
git commit -m "Mensagem explicando a mudança"
```

> 💡 Dica: escreva mensagens de commit curtas e descritivas.

---

## 🚀 Enviando Mudanças para o GitHub (Push)

Depois de realizar commits locais, envie as alterações para o seu repositório remoto:

```bash
git push origin main
```

Se estiver em outra branch:

```bash
git push origin nome-da-branch
```

Isso atualizará o seu repositório no GitHub com as mudanças feitas localmente.

---

## 🔄 Mantendo o Fork Atualizado (Upstream)

Para manter seu fork atualizado com o repositório original:

1. Adicione o repositório original como **upstream**:

```bash
git remote add upstream https://github.com/autor-original/repositorio.git
```

2. Busque as atualizações:

```bash
git fetch upstream
```

3. Atualize sua branch principal:

```bash
git merge upstream/main
```

4. Envie a atualização para o seu repositório remoto:

```bash
git push origin main
```


---

## 🧩 Criando um Pull Request (PR)

 <img width="1323" height="532" alt="{ECE7BF91-0955-44EE-8D75-983779E9510F}" src="https://github.com/user-attachments/assets/17043407-ccaa-4a3a-9644-1a6bdc55b797" />

Quando suas alterações estiverem prontas, você pode propor que sejam adicionadas ao repositório original.

### 🔹 Passos:

1. Vá até o repositório **original** no GitHub.
2. Clique em **“Compare & pull request”**.
3. Escreva uma descrição clara sobre suas alterações.
4. Clique em **“Create pull request”**.

Isso notificará o autor original, que poderá revisar e aceitar suas mudanças.

---

## 🧰 Resumo Visual do Fluxo

```text
Repositório Original
        │
        ▼
     Fork (GitHub)
        │
        ▼
     Clone (Local)
        │
        ▼
   Commit & Push (GitHub)
        │
        ▼
     Pull Request (Contribuição)
```

---

## 🏁 Conclusão

Agora você aprendeu o fluxo completo de contribuição usando **Git** e **Fork**:

* Fazer um fork de um repositório ✅
* Clonar para o seu computador ✅
* Editar e versionar com commits ✅
* Enviar alterações com push ✅
* Criar um pull request ✅

> 💬 “Contribuir é aprender colaborando — e cada commit é uma história registrada.”

---

### ✍️ Autor

**Marcola** — *Atividade prática sobre Git e Fork*
*Biologia Astronômica | 2025*
