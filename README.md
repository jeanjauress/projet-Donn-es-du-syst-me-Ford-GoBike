# Ford GoBike System Data Exploration
## par N'da kouassi jean jaures

## Aperçu
Exploration des données et communication des résultats du système Ford GoBike : ce document explore un ensemble de données contenant des informations sur les trajets individuels effectués dans un système de partage de vélos couvrant la grande région de la baie de San Francisco en 2019.

## Base de données

Les données consistent en des informations concernant 183.412 trajets effectués dans un système de partage de vélos couvrant la grande région de la baie de San Francisco en 2019. L'ensemble de données comprend 16 caractéristiques ('duration_sec', 'start_time', 'end_time', 'start_station_id', 'start_station_name' , 'start_station_latitude','start_station_longitude', 'end_station_id', 'end_station_name', 'end_station_latitude', 'end_station_longitude', 'bike_id', 'user_type','member_birth_year', 'member_gender', 'bike_share_for_all_trip'). L'ensemble de données peut être trouvé [ici](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv).
Après un nettoyage approprié des données, l'ensemble de données a été réduit et conçu en 12 colonnes, les nouvelles colonnes étant :

> day_of_week : pour stocker le numéro du jour de la semaine à partir de start_time.
> start_hour : pour stocker le numéro d'heure à partir de start_time.
> time_of_day : pour stocker l'heure du jour à partir de start_hour
> duration_min : pour stocker la durée en minutes.
> user_age : pour stocker l'âge de l'utilisateur du membre
> user_age_bin : âges groupés/regroupés pour l'exploration des tranches d'âge


## Résumé des résultats

L'utilisation des vélos par les abonnés et les clients était différente :

> Le jour de la semaine où la plupart des trajets sont effectués (jeudi) ne dépend PAS du fait qu'un utilisateur soit un abonné ou un client. Cependant, il a été découvert que les abonnés utilisaient principalement des vélos les jours ouvrables (du lundi au vendredi), tandis que l'utilisation des vélos par les clients était à peu près la même pendant toute la semaine, avec une augmentation considérable le samedi et le dimanche.
> En moyenne, les trajets des abonnés durent majoritairement (10-11) minutes, tandis que les clients durent majoritairement (23-24) minutes.
> Les trajets des clients étaient plus susceptibles de durer plus d'une heure par rapport aux abonnés.
> Les clients commencent souvent le voyage l'après-midi alors que les abonnés commencent principalement le matin suivi de l'après-midi.
> La plupart des trajets pour les abonnés ont commencé à 8 ou 17 heure. Alors que la plupart des trajets des clients ont commencé à 17 heure.
Durée moyenne du trajet en minutes :
> En moyenne, les balades du week-end (samedi et dimanche) ont duré plus longtemps que les autres jours.

## Informations clés pour la présentation

Pour la présentation :\
* Je me concentre uniquement sur l'heure de la journée et le jour de la semaine où la plupart des trajets sont effectués
* Combien de temps dure le trajet moyen ? et
* vérifiez si les résultats dépendent du fait qu'un utilisateur est un abonné ou un client.\
* La présentation a montré qu'il existe effectivement une dépendance entre la durée moyenne du trajet et le fait qu'un utilisateur soit un abonné ou un client. En moyenne, les trajets des clients ont duré plus longtemps que les trajets des abonnés tous les jours de la semaine et à toutes les heures de la journée


## Retour d'information

Si vous avez des commentaires, veuillez me contacter à ndakouassijj@gmail.com