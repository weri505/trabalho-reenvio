# trabalho-reenvio
import streamlit as st

st.title("Tabuada")
op = st.text_input(" Insira a operação desejada:\n [1] Adição\n [2] Subtração\n [3] Multiplicação\n [4] Divisão")

if op:
    op = int(op)

if op == 1:
    adicao = st.number_input('Digite qual número deseja ver a tabuada de adição:')
    num = 1
    while num <= 10:
        result = adicao + num
        st.write(f"{adicao} + {num} = {result}")
        num += 1

elif op == 2:
    sub = st.number_input('Digite qual número deseja ver a tabuada de subtração:')
    num = 1
    while num <= 10:
        result = sub - num
        st.write(f"{sub} - {num} = {result}")
        num += 1

elif op == 3:
    mult = st.number_input('Digite qual número deseja ver a tabuada de multiplicação:')
    num = 1
    while num <= 10:
        result = mult * num
        st.write(f"{mult} x {num} = {result}")
        num += 1

elif op == 4:
    div = st.number_input('Digite qual número deseja ver a tabuada de divisão:')
    num = 1
    while num <= 10:
        result = div / num
        st.write(f"{div} / {num} = {result}")
        num += 1
