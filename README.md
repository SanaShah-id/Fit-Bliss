# Fit-Bliss
To get bliss, be fit. This fitness App will help you out through physical training, nutrition, and diet, to get fit.

# Resource Description
Contains information about nutritional values including the meal plans, also provides an overall recommendation about what to eat.

# End points and Methods
GET healthyeating/{mealplan}
Get the mealplan by healthy eating.

# Parameters
## Path Parameters
| Path parameter | Description |
| ------ | ------ |
| {mealplan} | The idea for the meal you want to look up, Valid mealplan ideas are available from our site fitbliss.com. |

## Query string parameters
| Query string parameters | Required/ Optional | Description | Type |
| ------ | ------ | ------ | ------ |
| Breakfast | Optional | Count the total number of calories | Integer |
| Lunch | Optional | Count the total number of calories | Integer |
| Dinner | Optional | Count the total number of calories | Integer |
| Snacks | Optional | Count the total number of calories | Tnteger |

# Sample Request
```sh
curl -I -X GET "https://api.fitbliss.com/recepies/healthyeating/mealplan?appid=APIKEY&
```
(In the above code, replace 'APIKEY' with your actual key.)

# Sample Response
The following is a sample response from the **healthyeating/{mealplan}** endpoint:
```json
{
  "healthyeating": [
    {
      "mealplan": "Daily"
      "breakfast": {
        "8am" {
          "yogurt": "half cup",
          "Apple": 1,
          "Slice": 2,
          "Egg": 2,
          "Recommendation": "calory count is complete!"
        }
      }
      "lunch": {
        "1pm" {
          "vegtables": 1,
          "bread": 1,
          "chicken piece": 1,
          "salad": 1,
        }
      }
      "dinner": {
        "7pm" {
          "vegtables": 1,
          "bread": 1,
          "chicken piece": 1,
          "salad": 1,
        }
      }
      "snacks": {
        "5pm" {
          "tea": 1,
          "buscuit": 1,
        }
      }
    }
  ]
  }
```

# Response
The following table describes each item in the response.
| Response item | Description | Data type |
| yogurt | Semifluid fermented milk food | Object |
| Apple | Friut name, rich in Iron | Integer |
| Slice | A thin, broad piece of food | Integer |
| Egg | Rich in Protein | Integer |
| Vegetable | Edible product from plants | Integer |
| Bread | Wheat Chappati | Integer |
| Chicken piece | Meat rich in Protein | Integer |
| Salad | Edible product from plants | Integer |
| Tea | An aeromatic beverage | Integer |
| Buiscuit | Baked Product made from all purpose flour | Integer |
