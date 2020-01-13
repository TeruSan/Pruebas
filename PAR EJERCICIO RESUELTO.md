# Pc 0

* Destino: 1941610 
    * Defecto para todo lo demás: Default
* Máscara: 255.255.255.0 
    * Defecto para todo lo demás: 0.0.0.0
* Salto: Entrada directa 
    * Defecto para todo lo demás: 

# Router 0

* Destino: 194.16.2.0
    * 194.16.3.0
        + Default
* Mascara de red: 255.255.255.0
    * 255.255.255.0
        + 00.00
* Salto: Entrada directa
    * Entrada directa
        * Entrada directa

# Pc 1

* Destino: 194.16.4.0
    * 194.16.5.0
        * Default
* Máscara: 225.255.255.0
    * 225.255.255.0
        * 0.0.0.0
* Salto: Entrada directa
    * Entrada directa
        * 194.16.4.1

# Router 1

* Destino: 194.16.1.0
    * 194.16.2.0
        * 194.16.4.0
            * 194.16.3.0
                * 194.16.5.0
* Máscara: 225.255.255.0
    * 225.255.255.0
        * 225.255.255.0
            * 225.255.255.0
                * 225.255.255.0
* Salto: Entrada directa
    * Entrada directa
        * Entrada directa
            * 194.16.2.2
                * 194.16.4.2