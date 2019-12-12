# Motor mágneses terének intenzitás

# Ábra megrajzolása 

# Peremfeltételek megadása

x,y asszimetriája és szimmetriája miatt x irányban Neumann (g = 0, q=0), y irányban Dirichlet, a külső peremen is Dirichlet 

potenciális kérdés:  mit jelent g és q ebben az esetben? 

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

5200 az a maximálist érték amit a nemlineáris anyagnál elérhet a u értéke elméletben.

Érdemi változást nem lehet látni a két ábrán(lehet valamit rosszul csinálok). ur értékét tovább növelve a jelleg ugyanolyan mard  

Amennyiben a maximum(5200) érték helyett a minimumát(200) vesszük a nemlineáris anyagjellemző esetén, akkor jellegre van különbség. Emelett a az áramerősséget sokkal nagyobb értéknek vettem.

Az indukció nagysága nő, ezt a colorbar limitjén lehet látni.  

# Mit tapasztalunk ha finomítjuk?

Részletesebb ábrát kapunk, Inicializált meshnél a coil környékén állandónak tűnt a B, finomabb hálónál a két csúcsán sokkal nagyobb értékeket tapasztaltunk. Nem volt 'elkenődve' az ábra. 

Emellett sokkal nagyobb maximumok jelennek meg.
Tegyük fel hogy egy pontban van a maximum, körülötte kisebb értékek vannak. Amennyiben ezt egy háromszögre vesszük, és átlagoljuk, akkor kisebb érték lesz mint a maximum, amennyiben még nagyobbra vesszük, ahol még kisebb lesz az átlag, még kisebb értéket kapunk maximumnak. Minél kisebb mesh-et hozunk létre, annál jobban tudjuk lokalizálni a maximumot, és így a nagyság nő.
Jellegre a maximum a tekercs két végpontján lesz, amelyet egy 3d ábrán szemléltettünk is

