import matplotlib.pyplot as plt
from tamanho_variancia_grafico import *

signal_to_noise = 20


snr = 10**(signal_to_noise/10)
var_ruido = np.var(sinal) / snr

ruido = np.sqrt(var_ruido) * np.random.normal(0, 1, size=samples*ciclo)


ruido_sinal = sinal + ruido


calculo_sinal = 10*np.log10(np.var(ruido_sinal)/np.var(ruido))


fig, axs = plt.subplots(2, 1, figsize=(6, 5))

axs[0].plot(tempo, sinal)
axs[1].plot(tempo, ruido_sinal)

plt.tight_layout()
plt.show()
