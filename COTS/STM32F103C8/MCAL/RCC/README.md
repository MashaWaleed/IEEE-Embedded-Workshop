
# RCC DRIVER

This is a drive made to configure registers responsible for clock initilaization, control and reset


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

## MACRO Reference

 
 

