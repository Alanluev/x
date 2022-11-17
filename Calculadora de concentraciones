import streamlit as st
st.sidebar.subheader('Objetivo:')
st.sidebar.write('El objetivo de esta aplicación es facilitar a estudiantes de química el calcular concentraciones molares de soluciones.')
st.sidebar.subheader("Nombres de creadores:")
st.sidebar.markdown("-_Alan Pérez Luévano_")
st.sidebar.markdown("-_Luisana Aguilar Ornelas_")
st.sidebar.markdown('-_Janeth Tamara Reza Aguiñaga_')
st.sidebar.markdown('-_Kevin Jair Madrid_')


col1,col2=st.columns(2)

st.title('Calculadora de concentraciones ⚛')


tab1,tab2,tab3=st.tabs(['Inicio','Calculadora de Molaridad','Calculadora de Normalidad'])
with tab1:
  col1,col2=st.columns(2,gap="large")

  with col1:
    st.subheader(' ')
    st.subheader('_Molaridad:_ ')
    st.write('También mencionada como concentración molar, la molaridad señala qué tan concentrado está el soluto en la disolución. De este modo, la molaridad revela cuántos moles de soluto hay en cada litro de disolución.')
    st.text(' ')
    st.latex(r''' M= \frac{m}{PM*v}''')
   
    st.subheader(' ')

    st.write("m = masa del soluto (gr) ")
    st.write('PM= peso molecular del compuesto (L)')
    st. write('v = volumen de la solución .')
    st.header(' ')

  with col2:
    st.subheader(' ')
    st.subheader('_Normalidad:_ ')
    st.write('La normalidad es una medida de la concentración de una solución y se define como la relación entre los equivalentes de una sustancia y los litros de una solución. Los equivalentes se refieren a las cargas por mol de una sustancia.')
    st. latex(r''' N= \frac{m}{Pmeq*v}''')
    st.subheader(' ')

    st.write(' m = masa del soluto (gr)')
    st.write('Pmeq = peso miliequivalente del compuesto')
    st.write('v = volumen de la solución (ml)')

with tab2:
  st.subheader("Molaridad")

  compuesto = st.selectbox ('Escribe la formula quimica del compuesto',('NaOH','HCl','CH3COOH','H3PO4','HNO3','CaCl2','LiCl2','Mg3(PO4)2','Al(OH)3','Ca(OH)2','KCl','KOH','Na2SO4','Na2CO3','NaCl','kMnO4','HCOOH','NH3','H2SO4','C2H2O4','LiOH','Mg(OH)2','C6H8O7','C3H6O3','CH3COONa','KHP','CaCO3','MgSO4'))
  masa= st.number_input("Masa de Soluto (gr):")
  volumen= st.number_input("Volumen de Solución (L):",0.001)
  if compuesto== 'NaOH':
    PM=39.9971
  if compuesto== 'HCl':
    PM=36.4609
  if compuesto== 'CH3COOH':
    PM=60.0520
  if compuesto== 'H3PO4':
    PM=97.9952
  if compuesto== 'HNO3':
    PM=63.0128
  if compuesto== 'CaCl2':
    PM=110.9840
  if compuesto== 'LiCl2':
    PM=42.3940
  if compuesto== 'Mg3(PO4)2':
    PM=262.8577
  if compuesto== 'Al(OH)3':
    PM=78.0036
  if compuesto== 'Ca(OH)2':
    PM=74.0913
  if compuesto== 'KCl':
    PM=74.5513
  if compuesto== 'KOH':
    PM=56.1056
  if compuesto== 'Mg3(PO4)2':
    PM=262.8424
  if compuesto== 'Na2SO4':
    PM=142.04
  if compuesto== 'Na2CO3':
    PM=105.9884
  if compuesto== 'NaCl':
    PM=58.44
  if compuesto== 'KMnO4':
    PM=158.034
  if compuesto== 'HCOOH':
    PM=46.03
  if compuesto== 'NH3':
    PM=17.031
  if compuesto== 'NaOH':
    PM=39.9971
  if compuesto== 'H2SO4':
    PM=98.079
  if compuesto== 'C2H2O4':
    PM=90.03
  if compuesto== 'LiOH':
    PM=23.95
  if compuesto== 'Mg(OH)2':
    PM=39.997
  if compuesto== 'C6H8O7':
    PM=192.124
  if compuesto== 'C3H6O3':
    PM=128.1683
  if compuesto== 'CH3COONa':
    PM=82.0343
  if compuesto== 'KHP':
    PM=204.2212
  if compuesto== 'CaCO3':
    PM=100.0869
  if compuesto== 'NaOH':
    PM=39.997
  if compuesto== 'MgSO4':
    PM=120.366
    
  result=masa/(volumen*PM)
  result= round(result,5)
  if st.button("Calcular"):
    st.success(str(result)+' M')

with tab3:
  st. subheader("Normalidad")

 
  comp = st.selectbox ('Escribe la formula quimica del compuesto. ',('NaOH','HCl','CH3COOH','H3PO4','HNO3','CaCl2','LiCl2','Mg3(PO4)2','Al(OH)3','Ca(OH)2','KCl','KOH','Na2SO4','Na2CO3','NaCl','kMnO4','HCOOH','NH3','H2SO4','C2H2O4','LiOH','Mg(OH)2','C6H8O7','C3H6O3','CH3COONa','KHP','CaCO3','MgSO4'))
  m= st.number_input("Masa de Soluto (gr): ")
  v= st.number_input("Volumen de Solución (ml): ",0.001)

  if comp=="NaOH":
    PM=33.997
    eq=1
  if comp=="HCl":
    PM=36.4609
    eq=3
  if comp=="CH3COOH":
    PM=60.0520
    eq=1
  if comp=="H3PO4":
    PM=97.99252
    eq=2
  if comp=="HNO3":
    PM=63.0123
    eq=1
  if comp=="CaCl2":
    PM=1002940
    eq=6
  if comp=="LiCl":
    PM=42.3940
    eq=3
  if comp=="Mg3(PO4)2":
    PM=262.8577
    eq=2
  if comp=="Al(OH)3":
    PM=78.0036
    eq:1
  if comp=="Ca(OH)3":
    PM=74.0927
    eq=1
  if comp=="KCl":
    PM=74.5513
    eq=6
  if comp=="KOH":
    PM=56.1056
    eq=2
  if comp=="Mg3(PO4)2":
    PM=262.8424
    eq=2
  if comp=="Na2SO4":
    PM=142.04
    eq=1
  if comp=="Na2CO3":
    PM=105.9884
    eq=2
  if comp=="NaCl":
    PM=58.44
    eq=1
  if comp=="KMnO4":
    PM=158.034
    eq=1
  if comp=="HCOOH":
    PM=46.03
    eq=3
  if comp=="NH3":
    PM=17.031
    eq=2
  if comp=="NaOH":
    PM=39.9971
    eq=1
  if comp=="H2SO4":
    PM=98.079
    eq=2
  if comp=="C2H2O4":
    PM=90.03
    eq=1
  if comp=="LiOH":
    PM=23.95
    eq=2
  if comp=="Mg(OH)2":
    PM=39.997
    eq=2
  if comp=="C6H8O7":
    PM=192.124
    eq=1
  if comp=="C3H6O3":
    PM=128.1683
    eq=3
  if comp=="CH3COONa":
    PM=82.0343
    eq=1
  if comp=="KHP":
    PM=204.2212
    eq=2
  if comp=="CaCO3":
    PM=100.0869
    eq=1
  if comp=="MgSO4":
    PM=120.366
    eq=2
  


  resultado= m/((PM/(eq*1000))*v)
  resultado= round(resultado,5)
  if st.button('Calcular '):
    st.success(str(resultado)+" N")


  st.header(' ')
  
  st.subheader('Peso Miliequivalente')


  c = st.selectbox ('Escribe la formula quimica del compuesto ',('NaOH','HCl','CH3COOH','H3PO4','HNO3','CaCl2','LiCl2','Mg3(PO4)2','Al(OH)3','Ca(OH)2','KCl','KOH','Na2SO4','Na2CO3','NaCl','kMnO4','HCOOH','NH3','H2SO4','C2H2O4','LiOH','Mg(OH)2','C6H8O7','C3H6O3','CH3COONa','KHP','CaCO3','MgSO4'))
  if c=="NaOH":
    PM=33.997
    eq=1
  if c=="HCl":
    PM=36.4609
    eq=3
  if c=="CH3COOH":
    PM=60.0520
    eq=1
  if c=="H3PO4":
    PM=97.99252
    eq=2
  if c=="HNO3":
    PM=63.0123
    eq=1
  if c=="CaCl2":
    PM=1002940
    eq=6
  if c=="LiCl":
    PM=42.3940
    eq=3
  if c=="Mg3(PO4)2":
    PM=262.8577
    eq=2
  if c=="Al(OH)3":
    PM=78.0036
    eq=1
  if c=="Ca(OH)3":
    PM=74.0927
    eq=1
  if c=="KCl":
    PM=74.5513
    eq=6
  if c=="KOH":
    PM=56.1056
    eq=2
  if c=="Mg3(PO4)2":
    PM=262.8424
    eq=2
  if c=="Na2SO4":
    PM=142.04
    eq=1
  if c=="Na2CO3":
    PM=105.9884
    eq=2
  if c=="NaCl":
    PM=58.44
    eq=1
  if c=="KMnO4":
    PM=158.034
    eq=1
  if c=="HCOOH":
    PM=46.03
    eq=3
  if c=="NH3":
    PM=17.031
    eq=2
  if c=="NaOH":
    PM=39.9971
    eq=1
  if c=="H2SO4":
    PM=98.079
    eq=2
  if c=="C2H2O4":
    PM=90.03
    eq=1
  if c=="LiOH":
    PM=23.95
    eq=2
  if c=="Mg(OH)2":
    PM=39.997
    eq=2
  if c=="C6H8O7":
    PM=192.124
    eq=1
  if c=="C3H6O3":
    PM=128.1683
    eq=3
  if c=="CH3COONa":
    PM=82.0343
    eq=1
  if c=="KHP":
    PM=204.2212
    eq=2
  if c=="CaCO3":
    PM=100.0869
    eq=1
  if c=="MgSO4":
    PM=120.366
    eq=2

  R=PM/(eq*1000)
  R= round(R,5)
  if st.button(" Calcular"):
    st.success(str(R))
