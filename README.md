# rtrees
regression trees

IN the article of _(Local models-based regression trees for very short-term wind speed prediction A. Troncoso a, *, S. Salcedo-Sanz b, C. Casanova-Mateo c, J.C. Riquelme d, L. Prieto - SPAIN)_ a regression tree model is used for wind prediction for wind turbines, in which a regression model is used in each of the tree leaves. The question is how is this regression tree constructed? They say with the method of _(Luís Torgo LIACC - University of Porto - PORTUGAL)_ which grows a CART (Brieman 1984) tree with a different error function. Then it uses either a Kernel Regression or Linear Regression to make predictions on the new instances that fall within a tree node. Not very ground-breaking.

My idea of allowing diagonal splits seems more chupi-funny bunzy than the Iberian approach. :D

# lasso regression

seems good. minimize {Y-Xb} while trying |b1| + ... + |bm| < t, for t a regularization constant of our choosing. Note that previously the variables Y,Xi have been centered Y = Y-mean(Y), Xi = Xi - mean(Xi) and the covariates have been normalised, Xi1^2 + ... + XiN^2 = 1. Then this regression penalises big coefficients and favours coefficients that are zero.

The problem I see in this is that if a covariate has two symmetric extreme values like -0.5 and 0.5 while all the others are close to zero like 0.00001,0.00002, 0.00003, 0.00004,..., -0.0001, then the mean is 0 and the squared sum can be 1 but assuming that just the close to zero values are meaningful, the coefficient for this covariate would likely be of the order of 10^5 if the response Y is of the order of 1. This obviously creates a too big coefficient that won't be accepted if _t_ ~ 10^4 or smaller.

# optimization problem solution speed

[https://user-images.githubusercontent.com/28844803/34721941-1174200e-f545-11e7-9b37-9acca85ab337.jpg]

# asistencia a clase universitaria
Constitucion española -> Artículo 27.10 "Se reconoce la autonomía de las Universidades, en los términos que la ley establezca."

Ley Orgánica 6/2001, de 21 de diciembre, de Universidades BOE-A-2001-24515.

  Artículo 1.2 -> Son funciones de la Universidad al servicio de la sociedad:
        a) La creación, desarrollo, transmisión y crítica de la ciencia, de la técnica y de la cultura.
        b) La preparación para el ejercicio de actividades profesionales que exijan la aplicación 
          de conocimientos y métodos científicos y para la creación artística.
        c) La difusión, la valorización y la transferencia del conocimiento al servicio de la cultura, 
          de la calidad de la vida, y del desarrollo económico.
        d) La difusión del conocimiento y la cultura a través de la extensión universitaria y la 
         formación a lo largo de toda la vida.
         
  Artículo 6.2 -> Las Universidades públicas se regirán, además, por la Ley de su creación y por sus 
        Estatutos, que serán elaborados por aquéllas y, previo su control de legalidad, aprobados 
        por el Consejo de Gobierno de la Comunidad Autónoma. Si existieran reparos de legalidad, 
        las Universidades deberán subsanarlos, de acuerdo con el procedimiento previsto en sus 
        Estatutos,  y  someterlos  de  nuevo  a  la  aprobación  por  el  Gobierno  de  la  Comunidad 
        Autónoma.
        
 Artículo 42.4 -> Para facilitar la actualización de la formación y la readaptación profesionales y la plena 
y efectiva participación en la vida cultural, económica y social, el Gobierno, previo informe 
del Consejo de Universidades, regulará los procedimientos para el acceso a la universidad 
de quienes, acreditando una determinada experiencia laboral o profesional, no dispongan de 
la titulación académica legalmente requerida al efecto con carácter general. A este sistema 
de acceso, que permitirá el ingreso en cualquier universidad, centro y enseñanza, podrán 
acogerse también, en las condiciones que al efecto se establezcan, quienes, no pudiendo 
acreditar dicha experiencia, hayan superado una determinada edad


Estatut UPC 2012: 

Article 182. Estudiantes.
Son estudiantes de la Universitat Politècnica de Catalunya las personas matriculadas 
en las enseñanzas impartidas por la Universidad

HI ha un síndic de greuges!


# lebara calling prices with Dutch SIM

National prepaid pay as you go tariffs in the Netherlands 10=20 call credit
Mobile 	26ct/min
Landline 	12ct/min
Calls from Lebara to Lebara* 	   FREE*
SMS from Lebara to Lebara 	10ct/message
SMS 	21ct/message
Mobile internet (Charged per 100kB) 	49ct/MB
Start rate for calling landlines and mobiles (national or international calls) 	23ct/call
Voicemail (1233), rate per call 	20ct/call
