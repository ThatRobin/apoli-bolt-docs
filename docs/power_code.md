# Power Code

In Apoli-Beet, the structure for creating powers is rather different from the format usually used in Apoli, due to Apoli-Beets python-like syntax.

#### Creating a Function:

In order to create a basic power type in Apoli-Beet, you create an empty python function, like so:
```py
def launch_into_air():
    pass
```
This example creates an empty function called "launch_into_air".

#### Adding the Decorator:

Above this fuction, you will want to add something called a "decorator", in Apoli-Beet, the "power" decorator is what you add in order to specify that your function will be used in making powers.
=== "Apoli-Bolt"
    ```py
    @power("apoli:simple")
    def launch_into_air():
        pass
    ```
=== "Json"
    ```json
    {
        "type": "apoli:simple",
        "hidden": true
    }
    ```

#### Variable Specification:
The decorator you have created can work very similiarly to a json file. you can specify variables inside it, and they will be added to the json you made.
=== "Apoli-Bolt"
    ```py
    @power(type="apoli:launch", speed=5)
    def launch_into_air():
        pass
    ```
=== "Json"
    ```json
    {
        "type": "apoli:launch",
        "speed": 5,
        "hidden": true
    }
    ```

This method of writing powers can be used on its own in order to create any json file, in a similar way as you would using Apoli;
=== "Apoli-Bolt"
    ```py
    @power(
        type="apoli:active_self", 
        entity_action={
            type: "apoli:if_else",
            condition: {
                type: "apoli:on_fire"
            },
            if_action: {
                type: "apoli:extinguish"
            },
            else_action: {
                type: "apoli:set_on_fire",
                duration: 8
            }
        },
        cooldown=20
    )
    def launch_into_air():
        pass
    ```
=== "Json"
    ```json
    {
        "type": "apoli:active_self",
        "entity_action": {
            "type": "apoli:if_else",
            "condition": {
                "type": "apoli:on_fire"
            },
            "if_action": {
                "type": "apoli:extinguish"
            },
            "else_action": {
                "type": "apoli:set_on_fire",
                "duration": 8
            }
        },
        "cooldown": 20,
        "hidden": true
    }
    ```

#### Further Variables:
Apoli-Bolt also features some global variables, and can have much more complex syntax. All power files hold some global variables, particularly "entity" and "block", which are used in Actions and Conditions. This is used as part of Apoli-Bolts higher-level syntax.
=== "Apoli-Bolt"
    ```py
    @power(
        type="apoli:active_self", 
        cooldown=20
    )
    def launch_into_air():
        if entity.is_on_fire():
            entity.extinguish()
        else:
            entity.set_on_fire(8)
    ```
=== "Json"
    ```json
    {
        "type": "apoli:active_self", 
        "entity_action": {
            "type": "apoli:if_else",
            "condition": {
                "type": "apoli:on_fire"
            },
            "if_action": {
                "type": "apoli:extinguish"
            },
            "else_action": {
                "type": "apoli:set_on_fire",
                duration: 8
            }
        },
        "cooldown": 20
    }
    ```
