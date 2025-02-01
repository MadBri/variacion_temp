# ejercici_1

### main

import math

def temperatura(t, T0=5, Ts=40, k=0.45):
    return Ts + (T0 - Ts) * math.exp(-k * t)

def tiempo_para_temp_deseada(Td, T0=5, Ts=40, k=0.45):
    return -(math.log((Td - Ts) / (T0 - Ts)) / k)

if __name__ == "__main__":
    # Temperaturas a las 1, 5, 12 y 14 horas
    for horas in [1, 5, 12, 14]:
        print(f"Temperatura después de {horas} horas: {temperatura(horas):.2f} ºC")

    # Tiempo para que la temperatura sea 0.5ºC menos que la temperatura ambiente
    Td = Ts - 0.5
    tiempo = tiempo_para_temp_deseada(Td)
    print(f"Tiempo para alcanzar {Td} ºC: {tiempo:.2f} horas")

### Rama 1: `temperatura_horas`

Esta rama contiene el cálculo de la temperatura después de 1, 5, 12 y 14 horas.


import math

def temperatura(t, T0=5, Ts=40, k=0.45):
    return Ts + (T0 - Ts) * math.exp(-k * t)

if __name__ == "__main__":
    # Temperaturas a las 1, 5, 12 y 14 horas
    for horas in [1, 5, 12, 14]:
        print(f"Temperatura después de {horas} horas: {temperatura(horas):.2f} ºC")


### Rama 2: `tiempo_para_temp_deseada`



import math

def tiempo_para_temp_deseada(Td, T0=5, Ts=40, k=0.45):
    return -(math.log((Td - Ts) / (T0 - Ts)) / k)

if __name__ == "__main__":
    # Tiempo para que la temperatura sea 0.5ºC menos que la temperatura ambiente
    Td = Ts - 0.5
    tiempo = tiempo_para_temp_deseada(Td)
    print(f"Tiempo para alcanzar {Td} ºC: {tiempo:.2f} horas")
y

### Rama 3: `funciones_generales`


import math

def temperatura(t, T0=5, Ts=40, k=0.45):
    return Ts + (T0 - Ts) * math.exp(-k * t)

def tiempo_para_temp_deseada(Td, T0=5, Ts=40, k=0.45):
    return -(math.log((Td - Ts) / (T0 - Ts)) / k)

if __name__ == "__main__":
    # Temperaturas a las 1, 5, 12 y 14 horas
    for horas in [1, 5, 12, 14]:
        print(f"Temperatura después de {horas} horas: {temperatura(horas):.2f} ºC")

    # Tiempo para que la temperatura sea 0.5ºC menos que la temperatura ambiente
    Td = Ts - 0.5
    tiempo = tiempo_para_temp_deseada(Td)
    print(f"Tiempo para alcanzar {Td} ºC: {tiempo:.2f} horas")


