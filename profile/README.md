<p align="center">
  <img src="assets/logo-marsupi.png" alt="Marsupi" width="260">
</p>

<h3 align="center">O copiloto pedagógico da professora do 1º ano</h3>

<p align="center">
  Da foto da chamada à atividade certa para cada criança, com IA, sem diagnóstico e com a LGPD em primeiro lugar.
</p>

<p align="center">
  <a href="https://delta.fabricadesoftware.ifc.edu.br"><b>Acessar o Marsupi</b></a> ·
  <a href="https://github.com/Hackathon-Fabrica-2k26/Backend_template">Backend</a> ·
  <a href="https://github.com/Hackathon-Fabrica-2k26/Frontend_template">Frontend</a> ·
  <a href="https://github.com/Hackathon-Fabrica-2k26/Mobile_template">Mobile</a>
</p>

<p align="center">
  <sub>Hackathon Fábrica de Software 2026 · IFC Campus Araquari · desafio <i>“Do Zero à Autonomia: 24H com IA”</i></sub>
</p>

---

## O problema

Uma professora do 1º ano tem de 25 a 35 crianças na sala, cada uma num ritmo. Ela sabe que a IA poderia ajudar, mas:

- pergunta de forma genérica e recebe conselhos genéricos;
- não sabe que contexto dar para a IA, nem o que **não** pode dar (dados de crianças são protegidos pelo Art. 14 da LGPD);
- não tem tempo de adaptar a mesma atividade para cada criança.

## A proposta

O **Marsupi** conduz a professora do primeiro contato ao uso autônomo da IA no dia a dia da sala:

| Passo | O que a professora faz | O que o Marsupi faz |
|---|---|---|
| 1. Turma | Tira uma foto da lista de chamada | Lê os nomes, mostra a confiança de cada um e pede conferência dos duvidosos |
| 2. Atividade | Envia a atividade em PDF, DOCX ou foto | Extrai o texto e sugere título e descrição |
| 3. Versões | Clica em “Gerar versões” | Separa os alunos pela **habilidade a reforçar** (lista fixa do 1º ano, referência BNCC) e gera uma versão para cada grupo, sem mudar as questões |
| 4. Trabalhos | Fotografa os trabalhos entregues | Identifica de quem é cada um, aponta habilidades demonstradas e a reforçar e gera o relatório |
| 5. Acompanhamento | Abre o painel do aluno | Mostra relatórios, pontos de atenção (só com 3 ou mais trabalhos) e exporta tudo em PDF |

**Responsáveis entram sem criar conta:** a professora gera um link com código de uso único; o responsável dá o consentimento e pode enviar o laudo, que vira apenas necessidades e adaptações pedagógicas e é apagado logo depois.

## Telas

<p align="center"><sub>Telas do design (Figma). O produto publicado pode ter pequenas diferenças.</sub></p>

<table>
  <tr>
    <td width="50%"><img src="assets/sistema-inicio.png" alt="Início com as turmas da professora"><p align="center"><sub>Início: as turmas da professora</sub></p></td>
    <td width="50%"><img src="assets/sistema-nova-turma.png" alt="Nova turma a partir da foto da chamada"><p align="center"><sub>Nova turma pela foto da chamada</sub></p></td>
  </tr>
  <tr>
    <td><img src="assets/sistema-criar-atividade.png" alt="Criar atividade a partir de arquivo"><p align="center"><sub>Criar atividade (PDF, DOCX ou foto)</sub></p></td>
    <td><img src="assets/sistema-enviar-atividades.png" alt="Enviar os trabalhos dos estudantes"><p align="center"><sub>Enviar os trabalhos da turma</sub></p></td>
  </tr>
  <tr>
    <td><img src="assets/sistema-turma.png" alt="Página da turma"><p align="center"><sub>Página da turma</sub></p></td>
    <td><img src="assets/perfil-principal.png" alt="Perfil da professora"><p align="center"><sub>Perfil da professora</sub></p></td>
  </tr>
</table>

## Ética e privacidade

- **Não é ferramenta de diagnóstico.** O Marsupi nunca fala em TDAH, autismo, CID ou transtorno; fala em *habilidade a reforçar* e *necessidade pedagógica*.
- **Nenhum nome de criança vai para a IA.** Os textos são anonimizados antes; os nomes são casados no servidor.
- **Só com consentimento.** Aluno sem consentimento ativo do responsável não passa pela IA.
- **Arquivos não ficam guardados.** Fotos de trabalhos e laudos são lidos em memória e descartados.
- **A professora decide.** Toda versão e todo relatório passam pela revisão dela antes de ir para a sala.

## Tecnologia

| Parte | Stack |
|---|---|
| Backend | Python 3.13 · Django 5 · Django REST Framework · JWT · Google Gemini · ReportLab |
| Frontend | Vue 3 · Vuetify · TypeScript · Vite · Tailwind (utilitários) |
| Mobile | Flutter (APK gerado pelo GitHub Actions) |
| Deploy | GitHub Actions → Dokku (IFC Araquari) |

## Equipe

<table>
  <tr>
    <td align="center" width="16%"><a href="https://github.com/jonatasperaza"><img src="https://github.com/jonatasperaza.png" width="72" alt=""><br><sub><b>Jonatas Silva Peraza</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/IgorMMichels"><img src="https://github.com/IgorMMichels.png" width="72" alt=""><br><sub><b>Igor Michels</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/MatheusZenere"><img src="https://github.com/MatheusZenere.png" width="72" alt=""><br><sub><b>Matheus Vidal Zenere</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/Mateus2411"><img src="https://github.com/Mateus2411.png" width="72" alt=""><br><sub><b>Mateus Henrique da Silva</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/mklamaral"><img src="https://github.com/mklamaral.png" width="72" alt=""><br><sub><b>Mikael Amaral</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/Pedrojoseroza"><img src="https://github.com/Pedrojoseroza.png" width="72" alt=""><br><sub><b>Pedro José Oliveira da Roza</b></sub></a></td>
  </tr>
  <tr>
    <td align="center" width="16%"><a href="https://github.com/HigorAmaral"><img src="https://github.com/HigorAmaral.png" width="72" alt=""><br><sub><b>Higor do Amaral Fritz</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/Davi-Prussek"><img src="https://github.com/Davi-Prussek.png" width="72" alt=""><br><sub><b>Davi M. Prussek</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/kimnarciso"><img src="https://github.com/kimnarciso.png" width="72" alt=""><br><sub><b>Kimberlly Cristhinne Narciso</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/joaosantos86"><img src="https://github.com/joaosantos86.png" width="72" alt=""><br><sub><b>João Pedro</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/SaraKozoski"><img src="https://github.com/SaraKozoski.png" width="72" alt=""><br><sub><b>Sara Kozoski</b></sub></a></td>
    <td align="center" width="16%"><a href="https://github.com/danielhinsching"><img src="https://github.com/danielhinsching.png" width="72" alt=""><br><sub><b>Daniel dos Santos Hinsching</b></sub></a></td>
  </tr>
</table>

## Licença

© 2026 Equipe Marsupi. **Todos os direitos reservados.** O código e o design estão visíveis para avaliação do hackathon e para portfólio, mas **não podem ser copiados, modificados, redistribuídos nem usados** sem autorização por escrito da equipe. Veja [LICENSE](https://github.com/Hackathon-Fabrica-2k26/.github/blob/main/LICENSE).
