# QuickFixes

All minor issues I've faced and their solutions. Also contains things that I usually forget.

- [QuickFixes](#quickfixes)
    - [**PyTorch**](#pytorch)
    - [**MatPlotLib**](#matplotlib)

### **PyTorch**

> To select Device automatically

```python
DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
```

> TQDM iteration prints on new line. To fix this change the import statement to

```
from tqdm.auto import tqdm
```

### **MatPlotLib**

> To change figure size

```python
fig = plt.figure(figsize(width, height))
```

> Subplots, axis removal, title, plotting

```python
fig.add_subplot(MAX_ROWS, MAX_COLUMNS, index)
plt.axis("off")
plt.title("Title for the subplot")
plt.imshow(image_to_be_plotted)
```
