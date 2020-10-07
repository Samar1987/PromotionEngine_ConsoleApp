# PromotionEngine_ConsoleApp
To put my promotion engine console project with its unit test project for all 3 promotion types in given business requirement doc

Promotion Engine Console Application Description =>

(A) This application is currently having 3 Promotion types classes. But based upon business requirement we can add more promotion types without interacting\modifying an end user iterface of this application.
    (1) 3 of A's for 130
    (2) 2 of B's for 45
    (3) C & D for 30

(B) These promotion types are having an Interface - IProductPack which is being used to have common method need to be implemented in promotion type and product pack class to leverage [Composit Pattern].

(C) Application is having one service class - CartService with interface - ICartService implementation. This service class is responsible to perform 2 task.
      (1) Adding the products to oreder list based upon SKU Ids.
      (2) Calculating the total order value after applying 2 promotion type (currently these 2 promotion types are - (1) and (2) from above point (A))
      
(D) Service ICartService can be injected as dependency to an end user class to offer its services. So here [Interface Repository] patern is being implemented.


