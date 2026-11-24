# Projeto guiado — Computação Gráfica

Modelo do repositório do projeto guiado. Contém só a configuração (`.gitignore`, `.gitattributes`) e o modelo do registo de cada etapa (`docs/`). O projeto Unity é acrescentado por ti.

**Regra geral:** os ficheiros deste modelo ficam na **pasta do projeto Unity**, ou seja, a pasta que contém `Assets`, `Packages` e `ProjectSettings`.

---

## Opção A — Ainda não tenho repositório

1. Nesta página: **Use this template → Create a new repository**.
   - *Owner*: a tua conta. *Repository name*: por exemplo `cg-projeto-guiado`.
   - Seleciona **Private**. Depois, **Create repository**.
2. No **GitHub Desktop**: *File → Clone repository* → escolhe o repositório. Guarda-o numa pasta local, **não** sincronizada por OneDrive, Google Drive ou similar.
3. Copia para a pasta clonada as pastas **`Assets`, `Packages` e `ProjectSettings`** do projeto base indicado pelo docente. **Não** copies `Library`, `Temp`, `Logs` nem `UserSettings`.
4. No **Unity Hub**: *Add → Add project from disk* → seleciona a pasta clonada. Abre o projeto, confirma que a cena está correta e fecha o Unity.
5. No GitHub Desktop: escreve a mensagem "Projeto base" → **Commit to main** → **Push origin**.
6. Continua no ponto **"Partilhar com o docente"** mais abaixo.

## Opção B — Já tenho um repositório com o projeto

O objetivo é manter o histórico que já tens e acrescentar-lhe a configuração.

1. **O repositório tem de ser privado.** No github.com: *Settings → General → Danger Zone → Change repository visibility → Private*.
2. Nesta página: **Code → Download ZIP**. Do ZIP, copia para a pasta do projeto Unity:
   - `.gitignore` (substitui o teu, se já tiveres um);
   - `.gitattributes`;
   - a pasta `docs/`.
   No macOS, os ficheiros que começam por ponto estão escondidos no Finder. Usa *Cmd+Shift+.* para os mostrar.
3. **Se as pastas `Library`, `Temp`, `Logs`, `obj` ou `UserSettings` já foram enviadas para o GitHub** (aparecem na página do repositório):
   - fecha o Unity e **apaga essas pastas** no explorador de ficheiros. O Unity volta a criá-las da próxima vez que abrires o projeto, e pode demorar alguns minutos;
   - no GitHub Desktop vão aparecer muitos ficheiros apagados. É o esperado: faz commit com a mensagem "Remove pastas geradas pelo Unity".
4. Faz commit com a mensagem "Adiciona configuração do projeto guiado" → **Push origin**.
5. Os binários que já estavam no repositório ficam como estão. **Não** tentes convertê-los para LFS (`git lfs migrate`), porque isso reescreve o histórico. Os novos binários passam a ir para LFS automaticamente.
6. **Etapas que já terminaste:** no separador *History*, botão direito no commit que corresponde ao fim de cada etapa → *Create Tag…* → `etapa-01`, `etapa-02`, … → **Push origin**. Se não souberes qual é o commit, usa o mais recente e explica no registo da etapa.
7. Continua no ponto **"Partilhar com o docente"**.

---

## Partilhar com o docente
1. No github.com, no teu repositório: *Settings → Collaborators → Add people* → **`jpedev`**.
2. No IPB Virtual, na tarefa **Etapa 0**, submete o URL do repositório (por exemplo `https://github.com/<tua-conta>/cg-projeto-guiado`).

## Durante o trabalho
- Faz **commits frequentes** (pelo menos um por semana) com mensagens que digam o que mudou.
- Faz **Push** no fim de cada sessão. O trabalho que não está no GitHub não conta para a avaliação.
- Guarda a cena no Unity (*Ctrl+S*) antes de fazer commit.
- Não alteres o `.gitignore` nem o `.gitattributes`, e não retires o acesso ao docente.

## Fim de cada etapa
1. Copia `docs/etapa-00-modelo.md` para `docs/etapa-NN.md` e preenche-o.
2. Faz commit e push.
3. Separador *History* → botão direito no último commit → *Create Tag…* → **`etapa-NN`** (dois dígitos, por exemplo `etapa-03`) → **Push origin**.
4. No mesmo menu, usa **Copy SHA** para copiar o identificador do commit.
5. No IPB Virtual, submete:
   - o link `https://github.com/<tua-conta>/<repositório>/tree/etapa-NN`;
   - o SHA que copiaste.

**Não apagues nem movas tags.** O docente guarda uma cópia de cada tag no momento em que a vê, e qualquer alteração é detetada. Se te enganaste, cria uma tag nova (por exemplo `etapa-03-v2`) e submete-a no IPB Virtual.
