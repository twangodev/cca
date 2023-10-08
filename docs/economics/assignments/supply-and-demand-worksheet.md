# Supply and Demand Worksheet

1. Create a demand graph using the following table of values:

    | Price | Quantity |
    |-------|----------|
    | 10    | 500      |
    | 20    | 450      |
    | 30    | 400      |
    | 40    | 350      |
    | 50    | 300      |
    | 60    | 250      |
    | 70    | 200      |

    ```vegalite
    {
        "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
            "data": {
            "values": [
                {"Price": 10, "Quantity": 500},
                {"Price": 20, "Quantity": 450},
                {"Price": 30, "Quantity": 400},
                {"Price": 40, "Quantity": 350},
                {"Price": 50, "Quantity": 300},
                {"Price": 60, "Quantity": 250},
                {"Price": 70, "Quantity": 200}
            ]
        },
        "mark": "line",
        "encoding": {
        "x": {"field": "Quantity", "type": "quantitative", "title": "Quantity"},
        "y": {"field": "Price", "type": "quantitative", "title": "Price"}
        }
    }
    ```

2. Create a supply graph using the following table of values:

    | Price | Quantity |
    |-------|----------|
    | 10    | 200      |
    | 20    | 250      |
    | 30    | 300      |
    | 40    | 350      |
    | 50    | 400      |
    | 60    | 450      |
    | 70    | 500      |

    ```vegalite
    {
      "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
      "data": {
        "values": [
          {"Price": 10, "Quantity": 200},
          {"Price": 20, "Quantity": 250},
          {"Price": 30, "Quantity": 300},
          {"Price": 40, "Quantity": 350},
          {"Price": 50, "Quantity": 400},
          {"Price": 60, "Quantity": 450},
          {"Price": 70, "Quantity": 500}
        ]
      },
      "mark": "line",
      "encoding": {
        "x": {"field": "Quantity", "type": "quantitative", "title": "Quantity"},
        "y": {"field": "Price", "type": "quantitative", "title": "Price"}
      }
    }
    ```

3. Using the graphs above, what is the quantity demanded if the price is $10?

    From the demand graph, when the price is $10, the quantity demanded is 500.

4. Using the graphs above, what would be the quantity demanded at a price of $80? 

    It can be inferred that the quantity demanded would be lower than 200 if the price was $80.

5. Why is the demand at <span>$</span>80 lower than it is at $10?

    This reflects the basic law of demand which states that, all else being equal, as the price of a product increases, the quantity demanded falls; conversely, as the price falls, the quantity demanded rises. In this case, as price increases from $10 to $80, the quantity demanded decreases, indicating an inverse relationship between price and quantity demanded.

6. Using the graphs above creates a scenario which will cause each curve to shift (left and right). Draw NEW graphs and explain what the shifters are.

    1. A technological advancement in production reduces the cost of production. This would cause a rightward shift in the supply curve since suppliers can produce more at each price level.
    2. There's a decrease in consumers' income. This would cause a leftward shift in the demand curve, as consumers would buy less of the product at each price level due to reduced purchasing power.

    ```vegalite
    {
      "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
      "data": {
        "values": [
          {"Price": 10, "Quantity": 200, "Curve": "Original Supply"},
          {"Price": 20, "Quantity": 250, "Curve": "Original Supply"},
          {"Price": 30, "Quantity": 300, "Curve": "Original Supply"},
          {"Price": 40, "Quantity": 350, "Curve": "Original Supply"},
          {"Price": 50, "Quantity": 400, "Curve": "Original Supply"},
          {"Price": 60, "Quantity": 450, "Curve": "Original Supply"},
          {"Price": 70, "Quantity": 500, "Curve": "Original Supply"},
          {"Price": 10, "Quantity": 250, "Curve": "Shifted Supply"},
          {"Price": 20, "Quantity": 300, "Curve": "Shifted Supply"},
          {"Price": 30, "Quantity": 350, "Curve": "Shifted Supply"},
          {"Price": 40, "Quantity": 400, "Curve": "Shifted Supply"},
          {"Price": 50, "Quantity": 450, "Curve": "Shifted Supply"},
          {"Price": 60, "Quantity": 500, "Curve": "Shifted Supply"},
          {"Price": 70, "Quantity": 550, "Curve": "Shifted Supply"},
          {"Price": 10, "Quantity": 500, "Curve": "Original Demand"},
          {"Price": 20, "Quantity": 450, "Curve": "Original Demand"},
          {"Price": 30, "Quantity": 400, "Curve": "Original Demand"},
          {"Price": 40, "Quantity": 350, "Curve": "Original Demand"},
          {"Price": 50, "Quantity": 300, "Curve": "Original Demand"},
          {"Price": 60, "Quantity": 250, "Curve": "Original Demand"},
          {"Price": 70, "Quantity": 200, "Curve": "Original Demand"},
          {"Price": 10, "Quantity": 450, "Curve": "Shifted Demand"},
          {"Price": 20, "Quantity": 400, "Curve": "Shifted Demand"},
          {"Price": 30, "Quantity": 350, "Curve": "Shifted Demand"},
          {"Price": 40, "Quantity": 300, "Curve": "Shifted Demand"},
          {"Price": 50, "Quantity": 250, "Curve": "Shifted Demand"},
          {"Price": 60, "Quantity": 200, "Curve": "Shifted Demand"},
          {"Price": 70, "Quantity": 150, "Curve": "Shifted Demand"}
        ]
      },
      "mark": "line",
      "encoding": {
        "x": {"field": "Quantity", "type": "quantitative", "title": "Quantity"},
        "y": {"field": "Price", "type": "quantitative", "title": "Price"},
        "color": {"field": "Curve", "type": "nominal", "title": "Curve"}
      }
    }
    ```

    - The Original Supply Curve represents the initial supply before the technological advancement.
    - The Shifted Supply Curve shows how supply increased at each price point due to the technological advancement.
    - The Original Demand Curve represents the initial demand before the decrease in consumers' income.
    - The Shifted Demand Curve shows the decrease in quantity demanded at each price level after the reduction in consumers' income.