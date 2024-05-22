# Notas del proyecto. 


## Colocar linea en seguida de enlace en Navbar 
Con el **after** estamos volviendolo inlineblock para poderle dar una altura. Solo se le pone a la tablet

``` scss
&--crear {
            font-weight: 700;
            color: v.$primario;

            /* agregando linea divisora next to otros enlaces */
            @include m.tablet { 
                &::after {
                    content: '';
                    display: inlineblock;
                    height: 4rem;
                    border-right: 2px solid v.$grisClaro;
                    margin: 0 0 0 2rem;
                }
            }
        }
```