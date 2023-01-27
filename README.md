<h1>Créez et utilisez une base de données immobilière avec SQL</h1>
<h3>Scénario</h3>
<p>Vous êtes data analyst chez Laplace Immo, un réseau national d’agences immobilières. Le directeur général est sensible depuis quelque temps à l’importance des données, et il pense que l’agence doit se démarquer de la concurrence en créant un modèle pour mieux prévoir le prix de vente des biens immobiliers.&nbsp;</p>
<p>&nbsp;<img src="https://user.oc-static.com/upload/2020/11/24/16062363168182_image1.png" alt=""></p>
<p>Ce projet stratégique est appelé en interne le projet « DATAImmo ». La CTO de l’entreprise, Clara Daucourt, a la responsabilité de conduire le projet.</p>
<p>Dans ce cadre, elle vous a confié la modification de la base de données permettant de collecter les transactions immobilières et foncières en France. Vous utiliserez ensuite cette base pour analyser le marché et aider les différentes agences régionales à mieux accompagner leurs clients.</p>
<p>À votre arrivée ce matin, vous avez reçu un e-mail de la part de Clara, qui donne plus de détails sur ce qui est attendu de votre part.</p>
<p>&nbsp;</p>
<div class="oc-tableContainer"><table>
<tbody>
<tr>
<td>
<p><strong>Objet</strong> : Réunion de validation – Modification de la base de données.</p>
<p><strong>De </strong>: Clara</p>
<p><strong>À </strong>: Moi</p>
</td>
</tr>
<tr>
<td>
<p>Hello,&nbsp;</p>
<p>Afin d’avancer sur le projet DATAImmo, je prévois une première réunion pour valider la modification de la base de données.</p>
<p>Tu trouveras en pièce jointe un fichier zip avec les données suivantes :</p>
<ul>
<li>des données extraites du site open data des Demandes de valeurs foncières (DVF) ;</li>
<li>des données de l’INSEE avec les résultats des recensements de la population ;</li>
<li>des données de data.gouv sur les régions, avec le référentiel géographique français, communes, unités urbaines, aires urbaines, départements, académies, régions.</li>
</ul>
<p>&nbsp;</p>
<p>D’ici la réunion, j’aurais besoin de 2 choses de ta part :&nbsp;</p>
<ol>
<li>Il faut que tu prépares le dictionnaire des données en respectant le template en PJ pour répertorier et décrire les données importantes à stocker car nous avons omis de le faire. Il faut le remplir pour les trois fichiers de données.</li>
<li>Ensuite, peux-tu modifier le schéma relationnel en pièce-jointe pour qu’il prenne en compte les nouvelles données région et population ? Ça nous permettra de bien visualiser les différentes entités, associations et cardinalités de la base de données. Enfin, il faudra que tu me présentes ce nouveau schéma relationnel normalisé (Il doit suivre la norme 3NF) de la base de données qui donnera lieu à la création des nouvelles tables.&nbsp;</li>
</ol>
<p>On validera tout ça ensemble lors de notre réunion de validation, pour que tu puisses avancer sur la création de la base.</p>
<p>Je reste à ta disposition en cas de besoin.</p>
<p>Bien à toi,</p>
<p>Clara Daucourt</p>
<p><strong>CTO</strong></p>
</td>
</tr>
<tr>
<td>&nbsp;
<p><strong>Pièces jointes :&nbsp;</strong></p>
<ul>
<li><a href="https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Template_dico_donne%CC%81es.xlsx">Template du dictionnaire des données</a></li>
<li><a href="https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Donne%CC%81es-Immo.zip">Les données</a></li>
<li><a href="https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Sche%CC%81ma_relationnel_a%CC%80_refaire_et_modifier.jpg">Le schéma relationnel à recréer et modifier</a>&nbsp;</li>
</ul>
</td>
</tr>
</tbody>
</table></div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><img src="https://user.oc-static.com/upload/2022/06/14/16551936768392_DATA_deux-semaines-plus-tard.png" alt="">&nbsp;</p>
<p>Une fois cette première partie de votre travail effectuée, vous présentez votre travail à Clara qui valide votre schéma relationnel ainsi que le dictionnaire des données.&nbsp;</p>
<p>À ce stade du projet, vous pouvez valider avec votre mentor que votre conception est correcte avant d’aller plus loin.</p>
<p>Félicitations ! Elle vous envoie un e-mail à la suite de cette réunion.</p>
<div class="oc-tableContainer"><table>
<tbody>
<tr>
<td>
<p><strong>Objet</strong>: Validation du schéma relationnel et suite du projet</p>
<p><strong>De </strong>: Clara</p>
<p><strong>À </strong>: Moi</p>
</td>
</tr>
<tr>
<td>
<p>Hello,</p>
<p>Félicitations pour cette première étape de conception ! Comme on en a parlé en réunion ce matin, on est bons pour partir sur la modification de la base de données. Il faut maintenant que tu implémentes les tables dans la base de données en respectant ce qu’on s’est dit ce matin (cf. compte rendu de réunion en pièce jointe).</p>
<p>On a échangé en interne, et on pense qu’un outil comme SQLite est pertinent pour ce type d’implémentation. Si tu es plus à l’aise, tu peux essayer d’implémenter un outil comme mySQL ou postgreSQL.</p>
<p>Une fois que tu auras fait ça, tu pourras faire les requêtes pour extraire les données dont nous avons besoin. Pour ça, envoie-moi un document PDF avec tous les résultats des requêtes ainsi que la requête associée. Utilise des alias pour que ça soit plus lisible. Tu trouveras toutes les demandes auxquelles il faudra répondre dans le CR de réunion.</p>
<p>Une fois que tu auras terminé, on regardera tout ça ensemble pour voir ce que tu as réussi à tirer comme données.</p>
<p>Bon courage !</p>
<p>Clara Daucourt</p>
<p><strong>CTO</strong></p>
</td>
</tr>
<tr>
<td>&nbsp;<strong>Pièce jointe</strong> : <a href="https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/CR_re%CC%81union.pdf">Compte-rendu de réunion</a></td>
</tr>
</tbody>
</table></div>
<aside data-claire-semantic="information">
<p>Pour vous aider à avancer sur votre projet, nous vous proposons un <a href="https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Guide_etapes_cles+P3_DAN.pdf">guide des étapes clés</a> sur lequel vous pouvez baser votre travail. Chaque étape propose des recommandations à garder en tête, des problèmes à éviter et des ressources à utiliser.</p>
</aside>
<h3>&nbsp;Livrables&nbsp;</h3>
<ol>
<li>Dictionnaire des données.</li>
<li>Schéma relationnel normalisé modifié.&nbsp;</li>
<li>Base de données opérationnelle avec les données du 1er semestre 2020 (captures d’écran directement du système de gestion de base de données des tables construites).</li>
<li>Document avec les requêtes et les résultats (PDF).&nbsp;</li>
</ol>
