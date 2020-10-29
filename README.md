# Автоконтрастирование

Требуется написать алгоритм автоконтрастирования изображения:

```
def autocontrast(img: np.ndarray, white_percent: float, black_percent: float) -> np.ndarray:
```

Результат работы алгоритма должен соответствовать следующим требованиям (в порядке приоритета):
 
- black_percent - доля наиболее темных пикселей, которые нужно сделать черным (0) (например, 0.2)
- white_percent - доля наиболее светлых пикселей, которые нужно сделать белым (255) (например, 0.1)
- значения всех остальных пикселей нужно линейно растянуть на интервал (0, 255)

Если следующее требование выполнить невозможно (например, все пиксели после второго этапа уже черные или белые), алгоритм должен прекращать работу
