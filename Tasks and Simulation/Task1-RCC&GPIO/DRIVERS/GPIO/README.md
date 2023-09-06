
# GPIO DRIVER

This Driver was made to configure registers for certain functionalities regarding initialization of GPIO pins


## API Reference

### MCAL_GPIO_SetPinMode

```http
Std_ReturnType MCAL_GPIO_SetPinMode(u8 Copy_PortId, u8 Copy_PinId, u8 Copy_PinMode);
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Port`  `Pin`  `Mode`  | `u8` | Pre configured macros that desribe the layout of the pin |

| return | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Std_ReturnType ` | `u8` | describe if the function is implemented correctly |

Used to set if the pin is output or input and their respective modes.
 -
_________________________________
 
### MCAL_GPIO_SetPinValue

```http
Std_ReturnType MCAL_GPIO_SetPinValue(u8 Copy_PortId, u8 Copy_PinId, u8 Copy_PinValue);

```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Port`  `Pin`  `Value`  | `u8` | Pre configured macros that desribe the layout and value of the pin |

| return | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Std_ReturnType ` | `u8` | describe if the function is implemented correctly |

Used to write into an output pin with the specified pinValue, can be low or high.
 -
_________________________________
 

### MCAL_GPIO_GetPinValue

```http
Std_ReturnType MCAL_GPIO_GetPinValue(u8 Copy_PortId, u8 Copy_PinId, u8 *Copy_PinReturnValue);
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Port`  `Pin`  `Ptr`  | `u8` `u8 *` | Pre configured macros that desribe the layout and get value of the pin |

| return | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Std_ReturnType ` | `u8` | describe if the function is implemented correctly |

Used to read the value of an input pin and pass it be refrence to a param pointer
 -
_________________________________

## MACRO Reference

### GPIO_Port, GPIO_Values, GPIO_Pin  defgroups

#### These are made to interface the GPIO driver in a more readable and intuitive way, they each fall into their repsicitve, and appropiately named, API parameters !

![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/GPIO/Readme%20screens/macro%20ref%201.png?raw=true)

________________________________________________________________

### GPIO_InputMode, GPIO_OutputMode  defgroups

#### Selective macros for configuring GPIO pins direction and mode

![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/GPIO/Readme%20screens/macro%20ref%202.png?raw=true)

________________________________________________________________

### Private register mapping

#### Mapped registers of interest in the private section of the driver

![Screenshot](https://github.com/MashaWaleed/IEEE-Embedded-Workshop/blob/main/COTS/STM32F103C8/MCAL/GPIO/Readme%20screens/private.png?raw=true)
 
 

