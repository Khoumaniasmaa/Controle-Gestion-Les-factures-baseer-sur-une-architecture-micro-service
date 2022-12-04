# -Controle-Gestion-Les-factures-bas-e-sur-une-architecture-micro-service
Objectif :  
Créer une application basée sur une architecture micro-service qui permet de gérer les factures contenant des produits et appartenant à un client.
Travail à faire :
1.Créer le micro-service customer-service qui permet de gérer les client



2.Créer le micro-service inventory-service qui permet de gérer les produits

3. Créer la Gateway Spring cloud Gateway avec une Configuration statique du système de routage

![image](https://user-images.githubusercontent.com/84717947/202049977-16eaff6a-4e6c-4bec-8aee-73f671d516b6.png)

![image](https://user-images.githubusercontent.com/84717947/202050107-dd795b5c-62c7-4894-81bc-06f2b4033252.png)

4. Créer l'annuaire Eureka Discrovery Service

![202049977-16eaff6a-4e6c-4bec-8aee-73f671d516b6](https://user-images.githubusercontent.com/84717947/205496927-46fa6a34-1654-4ae1-a7ea-2659a7aa2d41.png)

5. Faire une configuration dynamique des routes de la gateway

5-1 Customers 

![image](https://user-images.githubusercontent.com/84717947/202050201-b95ba351-37ce-4e48-994b-f64635f4dec5.png)

5-2 Produits

![image](https://user-images.githubusercontent.com/84717947/202050249-3e0f9b2c-387c-44b0-8e07-73151297c458.png)

5-3Afficher customers par ID

![image](https://user-images.githubusercontent.com/84717947/202050295-559e544e-4da1-405d-a020-1be5e1828338.png)

6-4Produits par ID

![image](https://user-images.githubusercontent.com/84717947/202050329-3a574aea-cb06-40de-b0cc-874cd9bbcfe2.png)

6. Créer le service de facturation Billing-Service en utilisant Open Feign

7. Créer un client Web Angular (Clients, Produits, Factures)
    7.1-Listes des produits:

![Screenshot_1](https://user-images.githubusercontent.com/84717947/202864336-d3ed6e4c-b3f6-4e9a-8ee7-2ab5935bcc75.png)
     7.2- Listes des customers:

![Screenshot_2](https://user-images.githubusercontent.com/84717947/202864337-711f42f7-7dc0-4d90-948f-cd5d09b7404f.png)

     7.3-Les factures de chaque customer:

![Screenshot_3](https://user-images.githubusercontent.com/84717947/202864351-70f83694-6e47-41b0-90f5-5588603b58d4.png)

8. Déployer le serveur keycloak :

     - Créer un Realm!
     
     [Screenshot_3](https://user-images.githubusercontent.com/84717947/205497306-958af207-a2a5-43ba-b6be-c97538ccb1cf.png)
     
     - Créer un client à sécuriser
     
     ![Screenshot_4](https://user-images.githubusercontent.com/84717947/205497357-b130538b-d6d6-4a6f-b795-e668e9cb6ac8.png)

     - Créer des utilisateurs
     
     ![Screenshot_5](https://user-images.githubusercontent.com/84717947/205498112-f44ada28-f89c-49ba-b8fc-5619acc63b35.png)    

     - Créer des rôles
     
     ![Screenshot_6](https://user-images.githubusercontent.com/84717947/205498207-5e4517dd-c814-4428-b129-6231425fb372.png)

     - Affecter les rôles aux utilisateurs
     
     ![Screenshot_7](https://user-images.githubusercontent.com/84717947/205498321-f904a52e-9241-4e88-885a-f80bf3428dc6.png)

     ![Screenshot_8](https://user-images.githubusercontent.com/84717947/205498300-5e44a0a6-66ae-45e2-be83-9d0aac8ab3cd.png)

     ![Screenshot_9](https://user-images.githubusercontent.com/84717947/205498271-0836875d-db47-4108-87a2-a9467dfbb8fc.png)

     - Tester les différents modes d'authentification avec Postman en montrant les contenus de Access-Token, Refresh Token 
     
9. Sécuriser les micro-services et le frontend angular en déployant les adaptateurs Keycloak

9.1: Connecter a un user 

![Screenshot_10](https://user-images.githubusercontent.com/84717947/205498625-51779557-a9d6-4039-a58c-563654cf5cb9.png)

9.2 Product 

![Screenshot_11](https://user-images.githubusercontent.com/84717947/205498655-a4030cfa-a393-4123-82f4-7aff98298f87.png)

9.3: Customer 

![Screenshot_12](https://user-images.githubusercontent.com/84717947/205498688-5705e74d-c9d4-4b5e-8511-7b9474a96b05.png)

9.4 :facture:

![Screenshot_13](https://user-images.githubusercontent.com/84717947/205498702-ff2d7dcb-86bd-4d1d-9b74-66b7bee43907.png)

9.5-logout:

![Screenshot_14](https://user-images.githubusercontent.com/84717947/205498721-eb54b22a-ae4b-40b8-bbbd-bf6b9a43d035.png)

![Screenshot_15](https://user-images.githubusercontent.com/84717947/205498738-aa128020-e82e-40b2-9033-335a89010f6e.png)

