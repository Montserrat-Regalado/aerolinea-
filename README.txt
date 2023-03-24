+-------------+       +--------------+       +---------------+       +-----------+      +-----------+      +-----------+      +-------------+
|   Customer  |       |  Salesperson |       |     Product   |       |   Order   |      |   Review  |      |    Cart   |      |   Payment   |
+-------------+       +--------------+       +---------------+       +-----------+      +-----------+      +-----------+      +-------------+
| -id: int    |       | -id: int     |       | -id: int      |       | -id: int  |      | -id: int  |      | -id: int |      | -id: int    |
| -name: str  |       | -name: str   |       | -name: str   |       | -date: datetime |  | -rating: int |    | -items: List[Product] | | -amount: float|
| -email: str|       | -email: str |       | -price: float|       | -status: str |     | -comment: str|     | -customer_id: int    | | -method: str |
| -phone: str|       +--------------+       | -quantity: int|       | -customer_id: int | | -product_id: int | +-----------------------+ | -status: str |
+-------------+                            | -salesperson_id: int|  | -product_id: int | +-----------------------+                               +-------------+
| +get_id()  |                            | -category: str |       | -payment_id: int | | +add_item(product: Product)|                                       | +get_id()    |
| +get_name()|                            | -manufacturer: str |    | -total_amount: float | | +remove_item(product: Product)|                                     | +get_amount()|
| +get_email() |                          |                   |       |                     | | +get_items() |                                                            | +get_method()|
| +get_phone() |                          |                   |       |                     | | +set_status(status: str)|                                                             +-------------+
| +set_name(name: str)|                    | +get_id()       |       |                     | | +get_status() |                                                        
| +set_email(email: str)|                  | +get_name()     |       |                     | +------------------------+                                                      
| +set_phone(phone: str)|                  | +get_price()    |       |                     |                                                       
+-----------------------+                  | +get_category() |       |                     |                                                       
                                           | +get_manufacturer() |   +---------------------+                                                     
                                           | +set_name(name: str) |   | +get_id()     |                                                       
                                           | +set_price(price: float)| | +get_date()   |                                                       
                                           | +set_category(category: str)| +get_status() |                                                       
                                           | +set_manufacturer(manufacturer: str)| +get_customer_id()|                                                     
                                           +------------------x---------+ +get_product_id() |                                                 
                                                                             +get_payment_id()|                                                
                                                                             +get_total_amount()|                                              
                                                                             +set_status(status: str)|                                            
                                                                             +set_customer_id(customer_id: int)|                               
                                                                             +set_product_id(product_id: int)|                               
                                                                             +set_payment_id(payment_id: int)|                                
                                                                             +set_total_amount(total_amount: float)|                          
                                                                             +set_date(date: datetime)|                                        
                                                                             +set_items(items: List[Product])|                                
