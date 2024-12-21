# Conversor de Moneda y Temperatura 🌍🌡️  

Este proyecto es un conversor interactivo desarrollado en Java, que permite realizar conversiones entre diferentes divisas y unidades de temperatura de manera rápida y eficiente.  

![Interfaz Principal](https://github.com/user-attachments/assets/ab971f69-9cbb-466c-91d6-d5e7d1148971)  

En este proyecto puedes elegir manualmente qué opción prefieres: una conversión de divisas o de temperatura.  

![Opciones de Conversión](https://github.com/user-attachments/assets/4bc3f391-03d8-4e40-8430-62b708d968dd)  

## 📝 Descripción  
El **Conversor de Moneda y Temperatura** proporciona una solución sencilla para:  
- Convertir entre monedas internacionales con tasas predefinidas.  
- Convertir temperaturas entre las unidades más comunes: Celsius, Fahrenheit y Kelvin.  

## 📂 Estructura del Proyecto  
El repositorio incluye:  
- **`src`**: Contiene el código fuente del proyecto.  
- **Archivos de configuración**: Configuraciones necesarias para ejecutar y probar el programa.  
- **Documentación**: Instrucciones para usar y personalizar el conversor.  

## 🚀 Características  
1. **Conversor de Moneda**:  
   - Soporte para monedas populares como USD, EUR, COP, entre otras.  
   - Conversión precisa utilizando tasas predeterminadas.  

2. **Conversor de Temperatura**:  
   - Conversión entre grados Celsius, Fahrenheit y Kelvin.  
   - Validación de entrada para garantizar resultados correctos.  

3. **Interfaz amigable**: Interacción sencilla con mensajes claros para guiar al usuario.  



## 📂 Clase Destacada: `ConvertirMonedas`  
La clase `ConvertirMonedas` implementa métodos para realizar conversiones específicas de moneda:  

### Métodos Incluidos  
- **`ConvertirPesosADolares(double valor)`**  
  Convierte un monto en pesos colombianos (COP) a dólares estadounidenses (USD).  
  - Fórmula: `monedaDolar = valor / 3739.00`  
  - Redondeo a dos decimales para mayor precisión.  
  - Ejemplo de salida:  
    > "Tienes $ 50.27 Dólares"  

- **`ConvertirPesosAEuros(double valor)`**  
  Convierte un monto en pesos colombianos (COP) a euros (EUR).  
  - Fórmula: `monedaEuro = valor / 4050.48`  
  - Redondeo a dos decimales para mayor precisión.  
  - Ejemplo de salida:  
    > "Tienes $ 45.25 Euros"  

Ambos métodos utilizan `JOptionPane` para mostrar los resultados al usuario en una ventana emergente.  


   ```bash


public class ConvertirMonedas {

	public void ConvertirPesosADolares(double valor) {
		double monedaDolar = valor / 3739.00;
		monedaDolar = (double) Math.round(monedaDolar * 100d) / 100;
		JOptionPane.showMessageDialog(null, "Tienes $ " + monedaDolar + " Dolares");
	}

	public void ConvertirPesosAEuros(double valor) {
		double monedaEuro = valor / 4050.48;
		monedaEuro = (double) Math.round(monedaEuro * 100d) / 100;
		JOptionPane.showMessageDialog(null, "Tienes $ " + monedaEuro + " Euros");
	}

 
```

## 🛠️ Requisitos  
Para ejecutar este proyecto necesitas:  
- **Java Development Kit (JDK)** versión 8 o superior.  
- Un IDE compatible con Java (como IntelliJ IDEA, Eclipse o Visual Studio Code).  

## 💻 Cómo Ejecutar  
1. Clona este repositorio:  
   ```bash  
   git clone https://github.com/JUANSOTELO1709/ConversorMoneda  
