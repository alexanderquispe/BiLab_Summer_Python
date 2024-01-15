# group_6_ass_2_2024
# 1.1 Tuple
## 1. To access the first element, I used "[1]" and to access element 0 of the first element, I used "[0]"
tuple1 = ("Orange", [10, 20, 30], (5, 15, 25))
print(tuple1[1][0])

10

## 2. To access the last item, I used [2] for selecting location
tuple1 = ("Orange", [10, 20, 30], (5, 15, 25))
print(tuple1[2])

(5, 15, 25)

## 3. We change the word "Orange" replacing it with "pink grapefruit". In this case, it is posisble to replace the elements of the tuple1, because we are just renaming the composition of the first item of the tuple1 and keeping the rest items.

tuple1 = ("Orange", [10, 20, 30], (5, 15, 25))
tuple1 = ("pink grapefruit", [10, 20, 30], (5, 15, 25))
print(tuple1)

('pink grapefruit', [10, 20, 30], (5, 15, 25))

## 4. We apply the "Len" function to calculate the number of items
len(tuple1)
3

## 5. We use "map" to apply the sum list function to each sublist in tuple2
tuple2 = ([7, 8], [9, 1], [10, 7])
X = sum(map(sum, tuple2))
print(X)

42

## 6. We use "map" to apply the sum list function to each sublist in tuple3 but first, we need to find the half values of tuple2 
tuple3 = ([3.5, 4], [4.5, 0.5], [5, 3.5])
y= sum(map(sum , tuple3))
print(y)

21
# 1.2 List
## 1. Show the indices of the np.nan values in the f_list list. We want to see this output: The indices 0, 1, 4, 7 have np.nan values. Hint: Use print function and f-strings to insert the indices values.
nan_indices = [index for index, val in enumerate(f_list) if isinstance(val, float) and np.isnan(val)]
print(f"The indices {', '.join(map(str, nan_indices))} have np.nan values.")

The indices 0, 1, 4, 7 have np.nan values.

## 2. Replicate 4 times the values of the list p2_list. We expect an ouput like this: [ 2 , 3, 4, 5, 2 , 3, 4, 5, 2 , 3, 4, 5, 2 , 3, 4, 5]
p2_list = [2, 3, 4, 5]
replicated = p2_list * 4
print(replicated)

[2, 3, 4, 5, 2, 3, 4, 5, 2, 3, 4, 5, 2, 3, 4, 5]

## 3. Print the length of f_list.
print("f_list", len(f_list))

f_list 8

## 4. Print My teacher assistant is so boring. using text1 list.
text1 = ['My', 'teacher', 'assistant', 'is', 'so', 'boring.']
string = ' '.join(text1)
print(string)

My teacher assistant is so boring.

## 5. Print My TA is so boring, but is very funny. using text1 list.
text1.extend(['but', 'is', 'very', 'funny.'])
print(' '.join(text1))

My teacher assistant is so boring. but is very funny.

## 6. Print The max value of values1 is 86 and is located in the 0 index.
The min value of values1 is 0 and is located in the 7 index.

text1.extend(['but', 'is', 'very', 'funny.'])
print(' '.join(text1))

## 7. Get two lists: `names` and `last_names` using `last_and_name` list. 
last_and_name = [ "CORNEJO SANCHEZ, CHRISTIAN SANTOS", "ORELLANA QUISPE, CRISTIAN NASSER", "MORALES CHOQUEHUANCA, ANGELICA KARINA", "GUIMARAY RIBEYRO, JOSE ROBERTO", "CAMACHO GAVIDIA, ABEL FERNANDO", "TINTAYA ORIHUELA, MEIR ALVARO", "CHAVEZ MARTINEZ, JOSELIN ALEXANDRA", "FIGUEROA MURO, LEONEL ARTURO", "GOMEZ CRIBILLERO, JOSE FELIPE", "PALOMINO SEGUÍN, AFRANIA", "LUZON CUEVA, BIANCA MARIETTE", "SUAÑA ZEGARRA, ADRIAN ANDRE", "SOTO POMACHAGUA, DORKAS YOMIRA JHERMY", "FIORENTINO MARTINEZ, LADY ALY", "LAMA MAVILA, HECTOR ANDRE", "MEZA HINOJO, GUSTAVO", "LOZADA MURILLO, PERSEO MARCELO", "ZAMBRANO JIMENEZ, MIGUEL ALONZO", "JACOBS LUQUE, NICOLAS", "VIDAL VIDAL, ROCIO GABRIELA", "TORRES ANICAMA, JANE CAMILA", "LOPEZ ESTRADA, MARIA ELISA", "BOYCO ORAMS, ALEJANDRO", "DIAZ BERROSPI, KARLINE ROSMELI", "RIEGA ESCALANTE, STEPHY ROSARIO", "LEVANO TORRES, VALERIA CECILIA", "ESQUIVES BRAVO, SEBASTIAN RENATO", "PEREZ GONZALES, JUAN CARLOS", "OTERO MAGUIÑA, MARIANA", "CLAVO CAMPOS, ANDREA BRIZETH", "AGUILAR GARCIA, ERICK JOSUE", "CALDAS VELASQUEZ, JOSUE DANIEL", "SALAS NUÑEZ BORJA, FABIO MANUEL", "PIZARRO VILLANES, FERNANDA NICOLLE", "QUILLATUPA MORALES, ANGELA ADELINA", "HUANCAYA IDONE, CESAR DANTE", "CALVO PORTOCARRERO, GABRIELA ISABEL", "IBAÑEZ ABANTO, ANGEL MAURICIO", "MELÉNDEZ APONTE, JUAN DIEGO", "CRISTIAN SERRANO, ARONE", "HINOJOSA CAHUANA, PERCY ALBERTH", "ANGLAS GARCÍA, KEVIN ARTURO", "ALDAVE ACOSTA, CESAR ERNESTO", "NÚÑEZ HUAMÁN, CÉSAR AGUSTO", "OBREGON HUAMAN, DIANA EDITH", "SOTO PACHERRES, RODRIGO FRANCO", "INGARUCA RIVERA, GRETTEL ALEXANDRA", "ROJAS HUAMAN, ROSA ANGELA", "NEYRA SALAS, DANTE OMAR", "HUERTA ESPINOZA, YAJAIRA ALEXANDRA", "HUANCA MARTINEZ, JORGE ALBERTO", "FLORES CADILLO, ALEXIS" ]
names = list(map(lambda full_name: full_name.split(',')[1].lstrip(), last_and_name))
print("Names:", names)

Names: ['CHRISTIAN SANTOS', 'CRISTIAN NASSER', 'ANGELICA KARINA', 'JOSE ROBERTO', 'ABEL FERNANDO', 'MEIR ALVARO', 'JOSELIN ALEXANDRA', 'LEONEL ARTURO', 'JOSE FELIPE', 'AFRANIA', 'BIANCA MARIETTE', 'ADRIAN ANDRE', 'DORKAS YOMIRA JHERMY', 'LADY ALY', 'HECTOR ANDRE', 'GUSTAVO', 'PERSEO MARCELO', 'MIGUEL ALONZO', 'NICOLAS', 'ROCIO GABRIELA', 'JANE CAMILA', 'MARIA ELISA', 'ALEJANDRO', 'KARLINE ROSMELI', 'STEPHY ROSARIO', 'VALERIA CECILIA', 'SEBASTIAN RENATO', 'JUAN CARLOS', 'MARIANA', 'ANDREA BRIZETH', 'ERICK JOSUE', 'JOSUE DANIEL', 'FABIO MANUEL', 'FERNANDA NICOLLE', 'ANGELA ADELINA', 'CESAR DANTE', 'GABRIELA ISABEL', 'ANGEL MAURICIO', 'JUAN DIEGO', 'ARONE', 'PERCY ALBERTH', 'KEVIN ARTURO', 'CESAR ERNESTO', 'CÉSAR AGUSTO', 'DIANA EDITH', 'RODRIGO FRANCO', 'GRETTEL ALEXANDRA', 'ROSA ANGELA', 'DANTE OMAR', 'YAJAIRA ALEXANDRA', 'JORGE ALBERTO', 'ALEXIS']

last_names = list(map(lambda full_name: full_name.split(',')[0], last_and_name))
print("Last Names:", last_names)

Last Names: ['CORNEJO SANCHEZ', 'ORELLANA QUISPE', 'MORALES CHOQUEHUANCA', 'GUIMARAY RIBEYRO', 'CAMACHO GAVIDIA', 'TINTAYA ORIHUELA', 'CHAVEZ MARTINEZ', 'FIGUEROA MURO', 'GOMEZ CRIBILLERO', 'PALOMINO SEGUÍN', 'LUZON CUEVA', 'SUAÑA ZEGARRA', 'SOTO POMACHAGUA', 'FIORENTINO MARTINEZ', 'LAMA MAVILA', 'MEZA HINOJO', 'LOZADA MURILLO', 'ZAMBRANO JIMENEZ', 'JACOBS LUQUE', 'VIDAL VIDAL', 'TORRES ANICAMA', 'LOPEZ ESTRADA', 'BOYCO ORAMS', 'DIAZ BERROSPI', 'RIEGA ESCALANTE', 'LEVANO TORRES', 'ESQUIVES BRAVO', 'PEREZ GONZALES', 'OTERO MAGUIÑA', 'CLAVO CAMPOS', 'AGUILAR GARCIA', 'CALDAS VELASQUEZ', 'SALAS NUÑEZ BORJA', 'PIZARRO VILLANES', 'QUILLATUPA MORALES', 'HUANCAYA IDONE', 'CALVO PORTOCARRERO', 'IBAÑEZ ABANTO', 'MELÉNDEZ APONTE', 'CRISTIAN SERRANO', 'HINOJOSA CAHUANA', 'ANGLAS GARCÍA', 'ALDAVE ACOSTA', 'NÚÑEZ HUAMÁN', 'OBREGON HUAMAN', 'SOTO PACHERRES', 'INGARUCA RIVERA', 'ROJAS HUAMAN', 'NEYRA SALAS', 'HUERTA ESPINOZA', 'HUANCA MARTINEZ', 'FLORES CADILLO']

## 8. Give only the last names of students who do not have email. Use the `emails` and `last_names` list. 
last_and_name = [ "CORNEJO SANCHEZ, CHRISTIAN SANTOS", "ORELLANA QUISPE, CRISTIAN NASSER", "MORALES CHOQUEHUANCA, ANGELICA KARINA", "GUIMARAY RIBEYRO, JOSE ROBERTO", "CAMACHO GAVIDIA, ABEL FERNANDO", "TINTAYA ORIHUELA, MEIR ALVARO", "CHAVEZ MARTINEZ, JOSELIN ALEXANDRA", "FIGUEROA MURO, LEONEL ARTURO", "GOMEZ CRIBILLERO, JOSE FELIPE", "PALOMINO SEGUÍN, AFRANIA", "LUZON CUEVA, BIANCA MARIETTE", "SUAÑA ZEGARRA, ADRIAN ANDRE", "SOTO POMACHAGUA, DORKAS YOMIRA JHERMY", "FIORENTINO MARTINEZ, LADY ALY", "LAMA MAVILA, HECTOR ANDRE", "MEZA HINOJO, GUSTAVO", "LOZADA MURILLO, PERSEO MARCELO", "ZAMBRANO JIMENEZ, MIGUEL ALONZO", "JACOBS LUQUE, NICOLAS", "VIDAL VIDAL, ROCIO GABRIELA", "TORRES ANICAMA, JANE CAMILA", "LOPEZ ESTRADA, MARIA ELISA", "BOYCO ORAMS, ALEJANDRO", "DIAZ BERROSPI, KARLINE ROSMELI", "RIEGA ESCALANTE, STEPHY ROSARIO", "LEVANO TORRES, VALERIA CECILIA", "ESQUIVES BRAVO, SEBASTIAN RENATO", "PEREZ GONZALES, JUAN CARLOS", "OTERO MAGUIÑA, MARIANA", "CLAVO CAMPOS, ANDREA BRIZETH", "AGUILAR GARCIA, ERICK JOSUE", "CALDAS VELASQUEZ, JOSUE DANIEL", "SALAS NUÑEZ BORJA, FABIO MANUEL", "PIZARRO VILLANES, FERNANDA NICOLLE", "QUILLATUPA MORALES, ANGELA ADELINA", "HUANCAYA IDONE, CESAR DANTE", "CALVO PORTOCARRERO, GABRIELA ISABEL", "IBAÑEZ ABANTO, ANGEL MAURICIO", "MELÉNDEZ APONTE, JUAN DIEGO", "CRISTIAN SERRANO, ARONE", "HINOJOSA CAHUANA, PERCY ALBERTH", "ANGLAS GARCÍA, KEVIN ARTURO", "ALDAVE ACOSTA, CESAR ERNESTO", "NÚÑEZ HUAMÁN, CÉSAR AGUSTO", "OBREGON HUAMAN, DIANA EDITH", "SOTO PACHERRES, RODRIGO FRANCO", "INGARUCA RIVERA, GRETTEL ALEXANDRA", "ROJAS HUAMAN, ROSA ANGELA", "NEYRA SALAS, DANTE OMAR", "HUERTA ESPINOZA, YAJAIRA ALEXANDRA", "HUANCA MARTINEZ, JORGE ALBERTO", "FLORES CADILLO, ALEXIS" ]
emails = ["cscornejo@pucp.edu.pe", "orellana.cn@pucp.edu.pe", "karina.morales@pucp.edu.pe", "a20083223@pucp.pe", "abel.camacho@pucp.pe", "mtintaya@pucp.edu.pe", "joselin.chavez@pucp.edu.pe", "a20105737@pucp.pe", "jfgomezc@pucp.pe", "afrania.palomino@pucp.pe", "luzon.bianca@pucp.pe", "adrian.suanaz@pucp.pe", "soto.y@pucp.edu.pe", "a20132766@pucp.pe", "andre.lama@pucp.edu.pe", "gustavo.meza@pucp.edu.pe", "pmlozada@pucp.edu.pe", "m.zambranoj@pucp.edu.pe", "nicolas.jacobs@pucp.edu.pe", "gvidal@pucp.edu.pe", "jane.torres@pucp.edu.pe", "m.lopez@pucp.edu.pe", "alejandro.boyco@pucp.edu.pe", "a20167070@pucp.edu.pe", "riega.stephy@pucp.edu.pe", "vlevanot@pucp.edu.pe", "sesquives@pucp.edu.pe", "perez.juanc@pucp.edu.pe", "mariana.otero@pucp.edu.pe", "aclavo@pucp.edu.pe", "a20182474@pucp.edu.pe", "josue.caldas@pucp.edu.pe", "fabio.salas@pucp.edu.pe", "fernanda.pizarro@pucp.edu.pe", "aquillatupa@pucp.pe", "", "", "", "", "", "f0873079@pucp.edu.pe", "", "", "", "", "", "", "", "", "", "", "flores.alexis@pucp.edu.pe", ]
last_names = list(map(lambda full_name: full_name.split(',')[0], last_and_name))
combined_data = zip(last_names, emails)
last_names_no_email = [last_name for last_name, email in combined_data if email == '']
print("Last Names of Students without Email:", last_names_no_email)

Last Names of Students without Email: ['HUANCAYA IDONE', 'CALVO PORTOCARRERO', 'IBAÑEZ ABANTO', 'MELÉNDEZ APONTE', 'CRISTIAN SERRANO', 'ANGLAS GARCÍA', 'ALDAVE ACOSTA', 'NÚÑEZ HUAMÁN', 'OBREGON HUAMAN', 'SOTO PACHERRES', 'INGARUCA RIVERA', 'ROJAS HUAMAN', 'NEYRA SALAS', 'HUERTA ESPINOZA', 'HUANCA MARTINEZ']

# 1.3 Strings
## 1. Separate the words from str1 using the split method
      Join the words of Str1 with the join function
      Results are displayed with print
      
str1 = 'I am                          too                                                        old'
words = str1.split()
x = ' '.join(words)
print(x)

I am too old

## 2. To count the letters of str1, the 'len' function is used on the X created previously
len(x)
12

## 3. First we place the name blank spaces, then the .count formula that allows us to calculate the number of spaces in a certain section
Blank_spaces = str1.count(' ')
print(Blank_spaces)
85

len(str1) - len(x) -3
79

## 4. This code creates a list named positions by mapping the positions of the '@' symbol in each email address from the given emails list using the find('@') method. The resulting list, positions, holds the corresponding indices of the '@' symbol in each email address.
emails = ["cscornejo@pucp.edu.pe", "orellana.cn@pucp.edu.pe", "karina.morales@pucp.edu.pe", "a20083223@pucp.pe", "abel.camacho@pucp.pe", "mtintaya@pucp.edu.pe", "joselin.chavez@pucp.edu.pe", "a20105737@pucp.pe", "jfgomezc@pucp.pe", "afrania.palomino@pucp.pe", "luzon.bianca@pucp.pe", "adrian.suanaz@pucp.pe", "soto.y@pucp.edu.pe", "a20132766@pucp.pe", "andre.lama@pucp.edu.pe", "gustavo.meza@pucp.edu.pe", "pmlozada@pucp.edu.pe", "m.zambranoj@pucp.edu.pe", "nicolas.jacobs@pucp.edu.pe", "gvidal@pucp.edu.pe", "jane.torres@pucp.edu.pe", "m.lopez@pucp.edu.pe", "alejandro.boyco@pucp.edu.pe", "a20167070@pucp.edu.pe", "riega.stephy@pucp.edu.pe", "vlevanot@pucp.edu.pe", "sesquives@pucp.edu.pe", "perez.juanc@pucp.edu.pe", "mariana.otero@pucp.edu.pe", "aclavo@pucp.edu.pe", "a20182474@pucp.edu.pe", "josue.caldas@pucp.edu.pe", "fabio.salas@pucp.edu.pe", "fernanda.pizarro@pucp.edu.pe", "aquillatupa@pucp.pe"]
positions = list(map(lambda email: email.find('@'), emails))

print(positions)
[9, 11, 14, 9, 12, 8, 14, 9, 8, 16, 12, 13, 6, 9, 10, 12, 8, 11, 14, 6, 11, 7, 15, 9, 12, 8, 9, 11, 13, 6, 9, 12, 11, 16, 11]

## 5. This code creates a list named X using the map function and a lambda function. Each element in X corresponds to whether the substring ".edu." is present in the corresponding email address from the given emails list. The resulting list, X, contains Boolean values indicating the presence or absence of ".edu." in each email address.
emails = ["cscornejo@pucp.edu.pe", "orellana.cn@pucp.edu.pe", "karina.morales@pucp.edu.pe", "a20083223@pucp.pe", "abel.camacho@pucp.pe", "mtintaya@pucp.edu.pe", "joselin.chavez@pucp.edu.pe", "a20105737@pucp.pe", "jfgomezc@pucp.pe", "afrania.palomino@pucp.pe", "luzon.bianca@pucp.pe", "adrian.suanaz@pucp.pe", "soto.y@pucp.edu.pe", "a20132766@pucp.pe", "andre.lama@pucp.edu.pe", "gustavo.meza@pucp.edu.pe", "pmlozada@pucp.edu.pe", "m.zambranoj@pucp.edu.pe", "nicolas.jacobs@pucp.edu.pe", "gvidal@pucp.edu.pe", "jane.torres@pucp.edu.pe", "m.lopez@pucp.edu.pe", "alejandro.boyco@pucp.edu.pe", "a20167070@pucp.edu.pe", "riega.stephy@pucp.edu.pe", "vlevanot@pucp.edu.pe", "sesquives@pucp.edu.pe", "perez.juanc@pucp.edu.pe", "mariana.otero@pucp.edu.pe", "aclavo@pucp.edu.pe", "a20182474@pucp.edu.pe", "josue.caldas@pucp.edu.pe", "fabio.salas@pucp.edu.pe", "fernanda.pizarro@pucp.edu.pe", "aquillatupa@pucp.pe"]
X = list(map(lambda x: ".edu." in x, emails))

print(X)
[True, True, True, False, False, True, True, False, False, False, False, False, True, False, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, False]

## 6. The output is a list of lists, where each inner list includes the user part and a Boolean value indicating the presence of '@' in that user part. It's worth noting that the user extraction logic assumes a single dot before the domain and that the '@' symbol is always present in the user part.
emails = ["cscornejo@pucp.edu.pe", "orellana.cn@pucp.edu.pe", "karina.morales@pucp.edu.pe", "a20083223@pucp.pe", "abel.camacho@pucp.pe", "mtintaya@pucp.edu.pe", "joselin.chavez@pucp.edu.pe", "a20105737@pucp.pe", "jfgomezc@pucp.pe", "afrania.palomino@pucp.pe", "luzon.bianca@pucp.pe", "adrian.suanaz@pucp.pe", "soto.y@pucp.edu.pe", "a20132766@pucp.pe", "andre.lama@pucp.edu.pe", "gustavo.meza@pucp.edu.pe", "pmlozada@pucp.edu.pe", "m.zambranoj@pucp.edu.pe", "nicolas.jacobs@pucp.edu.pe", "gvidal@pucp.edu.pe", "jane.torres@pucp.edu.pe", "m.lopez@pucp.edu.pe", "alejandro.boyco@pucp.edu.pe", "a20167070@pucp.edu.pe", "riega.stephy@pucp.edu.pe", "vlevanot@pucp.edu.pe", "sesquives@pucp.edu.pe", "perez.juanc@pucp.edu.pe", "mariana.otero@pucp.edu.pe", "aclavo@pucp.edu.pe", "a20182474@pucp.edu.pe", "josue.caldas@pucp.edu.pe", "fabio.salas@pucp.edu.pe", "fernanda.pizarro@pucp.edu.pe", "aquillatupa@pucp.pe"]

positions = list(map(lambda email: email.find('@'), emails))

X = list(map(lambda x: ".edu." in x, emails))

users = []
for email in emails:
  user = email[:email.find(".")]
  has_at = "@" in user
  users.append([user, has_at])

print(users)

[['cscornejo@pucp', True], ['orellana', False], ['karina', False], ['a20083223@pucp', True], ['abel', False], ['mtintaya@pucp', True], ['joselin', False], ['a20105737@pucp', True], ['jfgomezc@pucp', True], ['afrania', False], ['luzon', False], ['adrian', False], ['soto', False], ['a20132766@pucp', True], ['andre', False], ['gustavo', False], ['pmlozada@pucp', True], ['m', False], ['nicolas', False], ['gvidal@pucp', True], ['jane', False], ['m', False], ['alejandro', False], ['a20167070@pucp', True], ['riega', False], ['vlevanot@pucp', True], ['sesquives@pucp', True], ['perez', False], ['mariana', False], ['aclavo@pucp', True], ['a20182474@pucp', True], ['josue', False], ['fabio', False], ['fernanda', False], ['aquillatupa@pucp', True]]
