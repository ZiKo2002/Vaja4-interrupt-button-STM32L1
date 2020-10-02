# Vaja4-interrupt-button-STM32L1
2.
b)	Ali lahko uporabite modro tipko za digitalni vhod kot interrupt (GPIO_EXT…). Če da, kateri pin je to? 
PA0
c)	Zapišite naslov izhodnih pinov za zeleno in modro LED: 
LD4 in LD3
3.
c)	Znotraj te funkcije zapišite ukaz za vklop/izklop zelene LED:
HAL_GPIO_TogglePin(GPIOC, LD3_Pin);
d)  Koliko znaša (v mili sekundah) zapisana zakasnitev, ki jo proizvede zanka for? 
2,8125 ms
e)  zapišite ukaz za utripanje modre LED:
HAL_GPIO_TogglePin(GPIOC, LD4_Pin);
f)	V to zanko dodajte ukaz za zakasnitev z funkcijo Delay iz knjižnice HAL, in sicer pol sekunde:
HAL_Delay(500);
4.
a)	Opazujte delovanje (utripanje modre LED). Kaj se zgodi, ko pritisnemo na modro tipko na STM32L1?
Ko pritisnemo modro tipko prižgemo/ugasnemo zeleno LED, modra led pa še naprej utripa.
b)	Ali pritisk na modro tipko vpliva na utripanje modre LED in zakaj?
Pritisk na modro tipko ne vpliva na utripanje modre LED zaradi interrupta, ki smo ga nastavili tipki.





