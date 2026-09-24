# pse-cours-2527

Révision des cours du parcours Programmeur Système d'Exploitation 2025-2027 (Linux, Windows Server, réseaux).

61 modules. **Module de formation autonome** : https://guiraudjb.github.io/pse-cours-2527/
(page `index.html` à la racine, `catalogue.json` limité à ce dépôt). Ses modules
apparaissent aussi dans l'application commune https://guiraudjb.github.io/PSE25-27/.

`index.html`, `sw.js` et les icônes sont une copie de la page commune
(`PSE25-27/`) : les modifier là-bas puis lancer `scripts/sync-web.py`, jamais ici.

## Séries

- **06** : Cours PSE 25-27
- **07** : Compléments Linux et réseau

## Organisation : un seul dossier pour le jeu et la page web

Tout est dans `batocera/pse-cours-2527/`, le dossier du jeu Batocera, copié tel quel
sur la console. La page web lit les **mêmes** fichiers (via GitHub Pages).

- `batocera/pse-cours-2527/data/` : `modules.json` (liste des modules) et, pour chaque
  module `<nom>` : `fiche/<nom>.txt`, `quizz/<nom>.csv`, `flashcard/<nom>.csv`,
  éventuellement `tp/<nom>.csv`, `icone/<nom>.png`, et les médias
  `podcast/<nom>.mp3`, `infographie/<nom>.png`, `chanson/<nom>.mp3` (+ paroles
  `.txt`), `fiche_audio/<nom>.mp3` (narration de la fiche).
- `batocera/pse-cours-2527/tts_assets/cache/<module>/` : audio des QCM (`quiz_N_ask`,
  `quiz_N_feedback_correct|incorrect`) et des flashcards (`flash_N_recto|verso`),
  joué par le jeu ET par la page web.
- `batocera/pse-cours-2527/*.py`, `pse-cours-2527.pygame`, `jeu.json`, `assets/` : le jeu.

## Outils (`batocera/`)

- `deploy.py` : copie le dossier du jeu sur la Batocera (SMB).
- `generate_tts_voicestudio.py` / `generate_fiche_audio_voicestudio.py` :
  génèrent l'audio (VoiceStudio local) directement dans le dossier du jeu.

Le moteur du jeu est commun à tous les dépôts : il se modifie dans le modèle
de l'espace de travail puis se synchronise, jamais ici.
