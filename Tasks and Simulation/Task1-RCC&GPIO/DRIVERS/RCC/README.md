
# RCC DRIVER

This is a driver made to configure registers responsible for clock initilaization, control and reset


## API Reference

### MCAL_RCC_InitSysClock

```http
  Std_ReturnType MCAL_RCC_InitSysClock(void);
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `void` | `void` |  |

| return | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Std_ReturnType ` | `u8` | describe if the function is implemented correctly |

Initialize system clock according to configurations.
 -
_________________________________
 
### MCAL_RCC_EnablePeripheral

```http
  Std_ReturnType MCAL_RCC_EnablePeripheral(u8 Copy_BusId, u8 Copy_PeripheralId);

```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `BusId` `Peripheral `      | `u8` | defined macros for Bus and peripheral in interface |

| return | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Std_ReturnType ` | `u8` | describe if the function is implemented correctly |

Enables a certain peripheral on any bus
 -
_________________________________
 

### MCAL_RCC_DisablePeripheral

```http
    Std_ReturnType MCAL_RCC_DisablePeripheral(u8 Copy_BusId, u8 Copy_PeripheralId);
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `BusId` `Peripheral `      | `u8` | defined macros for Bus and peripheral in interface |

| return | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Std_ReturnType ` | `u8` | describe if the function is implemented correctly |

Disables cetain peripheral using RCC ENR.
 -
_________________________________

## configuration MACRO Reference

### RCC_SYSCLK
- #### Used for configuring the source for the SYSCLK.
- #### There are three choices.
![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/RCC/read%20me%20screens/conf%20MACRO%20ref1.png?raw=true)
### RCC_PLL_SRC
- #### Used for configuring the source from PLL MUX.
- #### There are two choices.
![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/RCC/read%20me%20screens/conf%20MACRO%20ref2.png?raw=true)

### RCC_PLL_MUL
- #### Used for configuring PLL multiplier value.
- #### All possibilites stated by the TRM were implemented.
![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/RCC/read%20me%20screens/conf%20MACRO%20ref3.png?raw=true)

### External and Internal clock SPECS!
- #### Values of the SOCs internal and laid external clocks.
- #### Used for frequency calculations.
![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/RCC/read%20me%20screens/conf%20MACRO%20ref4.png?raw=true)
### RCC_CLK_BYPASS
- #### Determine the layout of the external clock (RC, RESONATOR).
- #### Two choices.
![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/RCC/read%20me%20screens/conf%20MACRO%20ref6.png?raw=true)

 
 

