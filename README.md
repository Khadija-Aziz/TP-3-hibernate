Exécution du projet : 

1.Structure du projet

<img width="1733" height="895" alt="Capture d’écran 2026-02-23 121100" src="https://github.com/user-attachments/assets/2247fbf2-1097-45c7-9bc3-56da433efa62" />

2.Exécution du App.java


Explication: Hibernate supprime d’abord les anciennes tables puis recrée automatiquement le schéma (utilisateurs, salles, réservations, équipements et la table de liaison ManyToMany). Les clés étrangères et contraintes sont bien générées.

1. Test des relations et cascad

2. Test de la suppression orpheline

Un utilisateur est créé avec deux réservations. Après suppression d’une réservation, le nombre passe de 2 à 1. La réservation supprimée n’existe plus en base, ce qui confirme que la gestion de la suppression fonctionne correctement.

3. Test de la relation ManyToMany

Des salles et des équipements sont créés puis associés.
Les tests montrent que :

-Une salle peut avoir plusieurs équipements.

-Un équipement peut appartenir à plusieurs salles.

-Supprimer une association ne supprime pas l’équipement de la base.

<img width="1830" height="822" alt="Capture d’écran 2026-02-23 114726" src="https://github.com/user-attachments/assets/92e767fe-7a71-4cbd-9a5e-95de6f7f7c9e" />
<img width="1830" height="886" alt="Capture d’écran 2026-02-23 114755" src="https://github.com/user-attachments/assets/8d88d7f9-c54b-4826-a0b9-458966838d7d" />
<img width="1821" height="795" alt="Capture d’écran 2026-02-23 114821" src="https://github.com/user-attachments/assets/8096a7e3-4e23-4651-a57f-6e921122a1f4" />
<img width="1819" height="888" alt="Capture d’écran 2026-02-23 114858" src="https://github.com/user-attachments/assets/f9f4a375-f700-4d42-924d-db5d42c70014" />
<img width="1817" height="885" alt="Capture d’écran 2026-02-23 114933" src="https://github.com/user-attachments/assets/ebb5853a-e3fb-46cc-be6c-3e7526bcaf21" />
<img width="1810" height="884" alt="Capture d’écran 2026-02-23 114955" src="https://github.com/user-attachments/assets/68d2268c-b4bf-47f7-a0a6-4722ea44e98b" />
<img width="1819" height="921" alt="Capture d’écran 2026-02-23 115050" src="https://github.com/user-attachments/assets/38b7aa95-9fd9-4f56-bafd-d2994bf280be" />
<img width="1820" height="885" alt="Capture d’écran 2026-02-23 115249" src="https://github.com/user-attachments/assets/2c843313-dfe5-43a7-ba2d-1b1f83bb068a" />
<img width="1821" height="874" alt="Capture d’écran 2026-02-23 115334" src="https://github.com/user-attachments/assets/8ff4d387-7078-47a9-b501-b7a2c4d843ea" />
<img width="1820" height="870" alt="Capture d’écran 2026-02-23 115718" src="https://github.com/user-attachments/assets/af723cf9-456c-46ff-8054-4ba9d2821414" />
<img width="1819" height="886" alt="Capture d’écran 2026-02-23 120333" src="https://github.com/user-attachments/assets/5ec3429b-98df-4efd-bbe3-521e9b129c5b" />
<img width="1824" height="879" alt="Capture d’écran 2026-02-23 120438" src="https://github.com/user-attachments/assets/28b3af0b-1f35-4175-8081-2f347b083e49" />
<img width="1815" height="892" alt="Capture d’écran 2026-02-23 120508" src="https://github.com/user-attachments/assets/cd5bf56c-d3b1-48e8-af4a-b1c913a57a68" />

<img width="1831" height="884" alt="Capture d’écran 2026-02-23 120551" src="https://github.com/user-attachments/assets/79d25d52-9577-4f8d-b180-12c1f4d38be8" />
<img width="1827" height="886" alt="Capture d’écran 2026-02-23 120631" src="https://github.com/user-attachments/assets/6058bb12-f2de-4e2d-bf1c-2977e0046149" />

<img width="1824" height="885" alt="Capture d’écran 2026-02-23 120704" src="https://github.com/user-attachments/assets/0291520b-3ad1-4253-a7c5-cfd94f35186d" />
<img width="1841" height="887" alt="Capture d’écran 2026-02-23 121008" src="https://github.com/user-attachments/assets/1cd93b3b-1bc3-4f03-97a6-a13b57798674" />
































