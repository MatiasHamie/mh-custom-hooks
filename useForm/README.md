# useForm

Ejemplo de uso:

```
    const initialForm = {
        name: '',
        age: 0,
        email: '',
    }

    const [ formValues, handleInputChange, reset ] = useForm( initialForm );
```

Maneja automaticamente el form con los campos que se necesiten, devolviendo los valores del mismo y funciones que modifican los valores segun se desee y un reset que vuelve todos los valores a los iniciales.
