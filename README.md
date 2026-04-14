Tout d'abord nous avons créé le dossier du projet grpc-tp, puis nous avons installé les bibliothèques avec la commande npm install @grpc/grpc-js @grpc/proto-loader

Après nous avons créé le fichier hello.proto et nous avons développé le fichier server.js pour créer le serveur gRPC où nous avons chargé le fichier hello.proto puis récupéré la définition du service.
Ensuite, nous avons implémenté la fonction sayHello créé un serveur gRPC, ajouté le service Greeter puis lancé le serveur sur l’adresse 0.0.0.0:50051.
Après nous avons créé le fichier client.js qui représente le client gRPC chargé de communiquer avec le serveur.
Nous avons de nouveau chargé le fichier hello.proto puis créé un client associé au service Greeter sur l’adresse localhost:50051.
Ensuite nous avons lancé le serveur avec la commande node server.js et  démarré le client avec node client.js:
<img width="413" height="63" alt="image" src="https://github.com/user-attachments/assets/f99f092d-fced-445b-b55a-e61d7d9bdc6f" />
<img width="450" height="65" alt="Capture" src="https://github.com/user-attachments/assets/5e9e1d27-e20a-4748-bb5a-fae48a5c0826" />
Aprés test avec Postman:créé une nouvelle requête gRPC, indiqué localhost:50051 comme hôte et importé le fichier hello.proto et  nous avons sélectionné le service Greeter et la méthode SayHello et  envoyé un objet JSON comme { "name": "fatma" }
<img width="1911" height="699" alt="lslslslsls" src="https://github.com/user-attachments/assets/308fe9c1-62c7-4441-9c5e-35d30be9595b" />


