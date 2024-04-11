You can stop read it


Dataset doc : https://hearthstonejson.com/docs/cards.html

Dataset : https://api.hearthstonejson.com/v1/195635/enUS/cards.collectible.json

Heartstone : Hearstone est un jeu de carte à collectioner au tour par tour. Au début de la partie chaque joueur selectionne une classe, un deck associé et commence avec 1 point de mana. le mana permet de jouer une carte selon le nombre de point indiquer. Le mana disponible augmentant d'un point par tour, jusqu’à atteindre un maximum de 10 points. Le joueur peut utiliser des serviteurs, des sorts ou des armes pour aire tomber les points de vie de l'adversaire à 0 et gagner la partie.

Carte à collectionner : Qui dit collection dit rareté. IL exise 5 niveaux de raretés : FREE, COMMUN, RARE, EPIC, LEGENDARY . Les cartes FREE sont les  carte disponible dès le début, elles sont fournis par le jeux. Le reste sont des stades de rareté dans l'orde croissant. 

Objectif : Notre but va être de prédire la rareté d'une carte de notre dataset.

Features du Dataset : 

- Artist : Nom de l'artiste de l'image de la carte
- cardClass : Classe a laquelle la carte appartient
- cost : Nombre nécéssaire de mana pour jouer la carte
- attack : Le nombre de dégats que peut infliger la carte (-1 pour les cartes qui ne peuvent pas infliger de dégat)
- health : Le nombre de dégats que peut recevoir la carte avant d'être détruite (complétement retirer du jeu, sauf contre indication)
- set : L'extension dans laquelle la carte est apparu ( écrit en entier ou abrégé)
- rarity : La rareté de la carte et également ce que l'ont essaie de prédire selon les autre feature
- mechanics : Chaque carte possede des effets qui ne sont pas unique mais s'applique différement selon chaque carte, certaine en on 2 ou 3 d'autres aucune (1 si la carte possède cette effet 0 sinon) c'est effet sont lister ici :
'is_SECRET', 'is_HEROPOWER_DAMAGE', 'is_RECEIVES_DOUBLE_SPELLDAMAGE_BONUS', 'is_INSPIRE', 'is_BATTLECRY', 'is_DEATHRATTLE', 'is_OVERHEAL', 'is_TRIGGER_VISUAL', 'is_InvisibleDeathrattle', 'is_COMBO', 'is_CHOOSE_ONE', 'is_AURA', 'is_OVERLOAD', 'is_CHARGE', 'is_DIVINE_SHIELD', 'is_FORGETFUL', 'is_SPELLPOWER', 'is_STEALTH', 'is_TAUNT', 'is_CANT_ATTACK', 'is_TOPDECK', 'is_DISCOVER', 'is_HONORABLEKILL', 'is_RUSH', 'is_WINDFURY', 'is_ImmuneToSpellpower', 'is_FRENZY', 'is_POISONOUS', 'is_LIFESTEAL', 'is_OUTCAST', 'is_MAGNETIC', 'is_AFFECTED_BY_SPELL_POWER', 'is_CANT_BE_TARGETED_BY_SPELLS', 'is_CANT_BE_TARGETED_BY_HERO_POWERS', 'is_GEARS','is_FINISH_ATTACK_SPELL_ON_DAMAGE', 'is_ECHO', 'is_FREEZE', 'is_GRIMY_GOONS', 'is_KABAL', 'is_JADE_GOLEM', 'is_JADE_LOTUS','is_TRADEABLE', 'is_ADJACENT_BUFF', 'is_ENRAGED', 'is_DEATH_KNIGHT', 'is_REBORN', 'is_START_OF_GAME', 'is_TWINSPELL', 'is_MULTIPLY_BUFF_VALUE', 'is_CORRUPT', 'is_SIDEQUEST', 'is_SILENCE', 'is_COLLECTIONMANAGER_FILTER_MANA_EVEN', 'is_COLLECTIONMANAGER_FILTER_MANA_ODD', 'is_INFUSE', 'is_MANATHIRST', 'is_DREDGE', 'is_COLOSSAL', 'is_SPELLBURST', 'is_OVERKILL', 'is_FORGE','is_TITAN', 'is_QUEST', 'is_EXCAVATE', 'is_QUICKDRAW'
