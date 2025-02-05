# Plane Game Engine Data Structures

Plane Game Engine uses JSON Schema for describing requirements for data
structures that are used in JSON assets.

The goal of this repository is to provide requirements for tools used in the
Plane Game Engine ecosystem.

[Online version](https://qbki.github.io/planeds/).

## An example of usage

You can refer to JSON Schema in your JSON assets through *$schema* keyword. For
instance, on the listing below you could see an example of invalid schema where
the color field must be an array type, but your editor or some other validation
tool will report an error.

```json
{
    "$schema": "https://raw.githubusercontent.com/qbki/planeds/refs/heads/main/v0/entities.json",
    "entities": {
        "7c4afd26-17e1-424c-bca6-ab2c9c8e4b66": {
            "color": {} // Incorrect type. Expected "array". (json)
            ...
        }
    }
}
```

## License

[MIT licensed](./LICENSE).
