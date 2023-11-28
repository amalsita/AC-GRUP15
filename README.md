# PROJECTE MACHINE LEARNING : MENTAL HEALTH CLUSTERING

## Participants
Amal El Hammoudi - 1608672

Àfrica Gamero - 1606033

Yasmin L'Harrak - 1603496

Èlia Vinyes - 1606019

## Introducció
Durant aquest projecte, ens endinsarem en el món del clustering aplicat a la salut mental en entorns laborals. La salut mental, que abasta el benestar cognitiu, conductual i emocional, ha emergit com un tema crucial en l'àmbit laboral, on alguns espais de treball es prioritza com un aspecte fonamental del benestar dels l'empleats, mentre que en altres, lamentablement, no se li atorga la deguda importància, donant lloc a estigmatització per part de companys i superiors cap a aquells que enfronten problemes mentals.

Per dur a terme aquest anàlisi, emprarem tècniques de clustering utilitzant Python, específicament en l'entorn de Jupyter.
hola

## Objectius

L'objectiu d'aquest projecte és identificar i classificar els empleats en dues categories distintes: aquells que treballen en un entorn laboral que brinda un sòlid suport a la salut mental, i aquells que lamentablement no compten amb aquest recolzament. Aquest enfocament ens permetrà comprendre millor quines dinàmiques laborals estan relacionades amb la salut mental i destacar la importància de crear entorns de treball que fomentin el benestar psicològic dels empleats. 


## Dataset

El dataset que utilitzem prové d' una enquesta sobre salut mental en l' entorn laboral.
Cada camp ofereix informació específica:

  **Timestamp**: Indica el moment en que es va realitzar l'enquesta.
  
  **Age**: Representa l'edat de l'enquestat, aquest camp haurà de tractar-se per evitar outliers.
  
  **Gender**:  Gènere de l'enquestat, el camp haurà de ser tractat per tal de homogeneïtzar els resultats.
  
  **Country**: País de residència, útil per identificar variacions geogràfiques.
  
  **State**: Aplicable només a enquestats als EEUU. Indica l'estat de residència per a anàlisi a nivell estatal.
  
  **Self-employed**: Informa si l'enquestat és autònom, rellevant per comprendre diferències en percepcions laborals.
  
  **Family_history**: Revela si hi ha antecedents familiars de malalties mentals.
  
  **Treatment**: Has buscat tractament per a una malaltia mental?
  
  **Work_interfere**: Si tens una malaltia mental, creus que interfereix amb la teva feina?
  
  **No_employees**: Quants empleats té la vostra empresa o organització?


## Starting Point

El punt inicial del nostre projecte comença en el tractament de les dades. A la columna de gènere, s'observa una diversitat d'entrades que representen el mateix terme però amb de diferent manera. Mitjançant un diccionari, s'ha realitzat manualment una unificació de termes per estandarditzar la informació.

Posteriorment, s'ha continuat amb l'anàlisi de valors nuls (Nans) en el conjunt de dades. A través d'una funció, hem calculat el porcentatge de nans per característica. En particular, hem identificat Nans en les característiques: State, work_interferee, self_employed i comentaris.


En el codi inicial, s'elimina l'edat, però nosaltres creiem que potser no hauria de ser descartada. Considerem que és un element que, tot i no ser aparentment rellevant ara, podria tenir una importància futura. Per tant, si en un moment posterior veiem que l'edat no és rellevant per al propòsit actual, tindrem en compte aquesta decisió i la seva exclusió del codi. El que s'ha fet és identificar les files on els valors són nuls i, substituir aquests Nans pel valor més freqüent de cada columna. Això ens permet omplir els buits amb els valors més comuns dins de cada característica per evitar la pèrdua d'informació rellevant en el conjunt de dades.

Es divideix en dos clusters: aquells que treballen en un entorn positiu pel que fa a la salut mental i aquells que no ho fan. Hem decidit explorar la possibilitat de segmentar-ho en diferents graus o nivells, com ara:

- Malaltia
- Potser
- Indiferent
- Possiblement
- No
  
Això ens permetrà comprendre les diferents percepcions o nivells de salut mental en relació amb l'entorn laboral, oferint una visió més detallada de les respostes dels participants en la classificació de la seva situació respecte a la salut mental en l'àmbit laboral.

## Arquitectura

## Versions

### Versió 1


### Versió 2

## Versió Final

## Conclusió
