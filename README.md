# Motor mágneses terének intenzitás

# Ábra megrajzolása 

# Peremfeltételek megadása

x,y szimmetriája és asszimetriája miatt x irányban Neumann (g = 0, q=0), y irányban Dirichlet, tényleges peremen dirichlet 

# PDE

ur -> coil és airgap u0

rotor és stator -> két eset:

  - u függ B-től, de B = rot(A) -> 2D miatt egyszerüsödik -> grad(A) : u = u0* 5000/grad(A) + 200)

  - lineáris -> 5200 (maximuma az előző esetnek)

# Mesh

Lehet finomítani, illetve adaptívan finomítani fontos helyeken(ahol nagy változásokat várunk)

# Plot 

Feladat szerint a mágneses indukció abszolútértékének sűrűségét és a fluxusvonalakat kellet -> flux density arrow és colormap

# Hogyan változik lineáris ur-re a plot? 

Érdemi változást nem lehet látni a két ábrán(lehet valamit rosszul csinálok) 

Az indukció nagysága nő, ezt a colorbar limitjén lehet látni.  

# Mit tapasztalunk ha finomítjuk?

Részletesebb ábrát kapunk, Inicializált meshnél a coil környékén állandónak tűnt a B, finomabb hálónál a két csúcsán sokkal nagyobb értékeket tapasztaltunk. Nem volt 'elkenődve' az ábra. 

Emellett sokkal nagyobb maximumok jelennek meg.
Tegyük fel hogy egy pontban van a maximum, körülötte kisebb értékek vannak. Amennyiben ezt egy háromszögre vesszük, és átlagoljuk, akkor kisebb érték lesz mint a maximum, amennyiben még nagyobbra vesszük, ahol még kisebb lesz az átlag, még kisebb értéket kapunk maximumnak.

