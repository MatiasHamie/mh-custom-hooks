# useFetch

Ejemplo de uso:

```
    const url = 'endpoint de una API';

    // Valor por defecto
    const {data: null, loading: true, error: null} = useFetch(url);
```

Cuando se carga por primera vez, el useEffect inicializa un booleano "isMounted" en true y se guarda la referencia con useRef del mismo.

En cualquier momento que se deja de utilizar el hook, se pasa el booleano "isMounted" a false.

Entonces antes de actualizar el estado de la data traida de la API, verifica que este isMounted en true, para que no haya colisiones de datos / mas de una peticion accidental.
