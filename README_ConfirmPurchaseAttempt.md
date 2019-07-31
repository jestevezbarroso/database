# AmountEngineService. ConfirmPurchaseAttempt

All requests regarding the **ConfirmPurchaseAttempt** service are listed below:

- [All parameters](#all-parameters)
- [No adjustments](#no-adjustments)
- [Neither promotion codes nor any adjustments](#neither-promotion-codes-nor-any-adjustments)
- [No promotion codes](#no-promotion-codes)
- [No lines](#no-lines)
- [Neither lines nor any adjustments](#neither-lines-nor-any-adjustments)
- [No adjustments (Manual-order)](#no-adjustments-manual-order)
- [Neither adjustments (Manual-order) nor promotion code](#neither-adjustments-manual-order-nor-promotion-code)
- [Neither lines nor adjustments (Manual-order)](#neither-lines-nor-adjustments-manual-order)
- [Neither promotion code nor lines](#neither-promotion-code-nor-lines)
- [Neither promotion code nor lines nor adjustments](#neither-promotion-code-nor-lines-nor-adjustments)
- [No adjustments belonging to lines](#no-adjustments-belonging-to-lines)
- [Neither adjustments belonging to lines nor promotion code](#neither-adjustments-belonging-to-lines-nor-promotion-code)
- [Neither adjustments nor promotion code nor adjustments belonging to lines](#neither-adjustments-nor-promotion-code-nor-adjustments-belonging-to-lines)
- [No order id](#no-order-id)
- [No store id](#no-store-id)
- [No delivery](#no-delivery)

## All parameters
### Request
- DEV
```sh		
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh		
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh		
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh		
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```

### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6350"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6100"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-541"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1459"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-458"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        },
        "description": {
          "value": "short description in Spanish"
        },
        "type": "GENERIC",
        "code": {
          "value": "PROMOTION_CODE"
        }
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6750"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## No adjustments
### Request

- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6550"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        },
        "description": {
          "value": "short description in Spanish"
        },
        "type": "GENERIC",
        "code": {
          "value": "PROMOTION_CODE"
        }
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6950"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
## Neither promotion codes nor any adjustments
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6470"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-80"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "170"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-80"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6950"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## No promotion codes
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6270"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6100"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-80"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "170"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-541"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1459"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-458"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      },
      {
        "amount": {
          "value": {
            "value": "-80"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6750"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
## No lines
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE-LT
Excerpt from the exception happend
```json
{
  "payload": null,
  "status": {
    "code": "UNKNOWN",
    "description": null,
    "cause": {
      "cause": {
        "cause": {
          "cause": null,
          "stackTrace": [
            {
              "methodName": "get",
              "fileName": "Optional.java",
              "lineNumber": 135,
              "className": "java.util.Optional",
              "nativeMethod": false
            },
            {
              "methodName": "calculate",
              "fileName": "TotalListPriceCalculatorImpl.java",
              "lineNumber": 69,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.order.TotalListPriceCalculatorImpl",
              "nativeMethod": false
            },
            {
              "methodName": "execCalculators",
              "fileName": "CalculatorChain.java",
              "lineNumber": 84,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.CalculatorChain",
              "nativeMethod": false
            },
            {
              "methodName": "calculateCart",
              "fileName": "ProcessManagementServiceImpl.java",
              "lineNumber": 224,
              "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
              "nativeMethod": false
            }
          ]
        }
      }
    }
  }
}
```
## Neither lines nor any adjustments
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT
```json

```
- PRE-LT
Excerpt from the exception happend
```json
{
  "payload": null,
  "status": {
    "code": "UNKNOWN",
    "description": null,
    "cause": {
      "cause": {
        "cause": {
          "cause": null,
          "stackTrace": [
            {
              "methodName": "get",
              "fileName": "Optional.java",
              "lineNumber": 135,
              "className": "java.util.Optional",
              "nativeMethod": false
            },
            {
              "methodName": "calculate",
              "fileName": "TotalListPriceCalculatorImpl.java",
              "lineNumber": 69,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.order.TotalListPriceCalculatorImpl",
              "nativeMethod": false
            },
            {
              "methodName": "execCalculators",
              "fileName": "CalculatorChain.java",
              "lineNumber": 84,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.CalculatorChain",
              "nativeMethod": false
            },
            {
              "methodName": "calculateCart",
              "fileName": "ProcessManagementServiceImpl.java",
              "lineNumber": 224,
              "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
              "nativeMethod": false
            }
          ]
        }
      }
    }
  }
}
```
## No adjustments (Manual-order)
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6550"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        },
        "description": {
          "value": "short description in Spanish"
        },
        "type": "GENERIC",
        "code": {
          "value": "PROMOTION_CODE"
        }
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6950"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## Neither adjustments (Manual-order) nor promotion code
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6470"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-80"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "170"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "72"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-80"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6950"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-300"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6700"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-83"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1917"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-84"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1916"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-25"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "475"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
## Neither lines nor adjustments (Manual-order)
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE-LT
Excerpt from the exception happend
```json
{
  "payload": null,
  "status": {
    "code": "UNKNOWN",
    "description": null,
    "cause": {
      "cause": {
        "cause": {
          "cause": null,
          "stackTrace": [
            {
              "methodName": "get",
              "fileName": "Optional.java",
              "lineNumber": 135,
              "className": "java.util.Optional",
              "nativeMethod": false
            },
            {
              "methodName": "calculate",
              "fileName": "TotalListPriceCalculatorImpl.java",
              "lineNumber": 69,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.order.TotalListPriceCalculatorImpl",
              "nativeMethod": false
            },
            {
              "methodName": "execCalculators",
              "fileName": "CalculatorChain.java",
              "lineNumber": 84,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.CalculatorChain",
              "nativeMethod": false
            },
            {
              "methodName": "calculateCart",
              "fileName": "ProcessManagementServiceImpl.java",
              "lineNumber": 224,
              "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
              "nativeMethod": false
            }
          ]
        }
      }
    }
  }
}
```

## Neither promotion code nor lines
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: d3870915-ce74-4187-a88d-632db71d329d' \
  -H 'cache-control: no-cache' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: d3870915-ce74-4187-a88d-632db71d329d' \
  -H 'cache-control: no-cache' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: d3870915-ce74-4187-a88d-632db71d329d' \
  -H 'cache-control: no-cache' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: d3870915-ce74-4187-a88d-632db71d329d' \
  -H 'cache-control: no-cache' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE-LT
Excerpt from the exception happend
```json
{
  "payload": null,
  "status": {
    "code": "UNKNOWN",
    "description": null,
    "cause": {
      "cause": {
        "cause": {
          "cause": null,
          "stackTrace": [
            {
              "methodName": "get",
              "fileName": "Optional.java",
              "lineNumber": 135,
              "className": "java.util.Optional",
              "nativeMethod": false
            },
            {
              "methodName": "calculate",
              "fileName": "TotalListPriceCalculatorImpl.java",
              "lineNumber": 69,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.order.TotalListPriceCalculatorImpl",
              "nativeMethod": false
            },
            {
              "methodName": "execCalculators",
              "fileName": "CalculatorChain.java",
              "lineNumber": 84,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.CalculatorChain",
              "nativeMethod": false
            },
            {
              "methodName": "calculateCart",
              "fileName": "ProcessManagementServiceImpl.java",
              "lineNumber": 224,
              "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
              "nativeMethod": false
            }
          ]
        }
      }
    }
  }
}
```
## Neither promotion code nor lines nor adjustments
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

- PRE-LT
Excerpt from the exception happend
```json
{
  "payload": null,
  "status": {
    "code": "UNKNOWN",
    "description": null,
    "cause": {
      "cause": {
        "cause": {
          "cause": null,
          "stackTrace": [
            {
              "methodName": "get",
              "fileName": "Optional.java",
              "lineNumber": 135,
              "className": "java.util.Optional",
              "nativeMethod": false
            },
            {
              "methodName": "calculate",
              "fileName": "TotalListPriceCalculatorImpl.java",
              "lineNumber": 69,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.order.TotalListPriceCalculatorImpl",
              "nativeMethod": false
            },
            {
              "methodName": "execCalculators",
              "fileName": "CalculatorChain.java",
              "lineNumber": 84,
              "className": "com.inditex.mecc.appmicmeccameng.model.calculator.CalculatorChain",
              "nativeMethod": false
            },
            {
              "methodName": "calculateCart",
              "fileName": "ProcessManagementServiceImpl.java",
              "lineNumber": 224,
              "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
              "nativeMethod": false
            }
          ]
        }
      }
    }
  }
}
```
## No adjustments belonging to lines
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6650"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-600"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-458"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1542"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-458"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "0"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "PromoCode_DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        },
        "description": {
          "value": "short description in Spanish"
        },
        "type": "GENERIC",
        "code": {
          "value": "PROMOTION_CODE"
        }
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "PromoCode_DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "7050"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-200"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6800"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-58"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1942"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## Neither adjustments belonging to lines nor without promotion code
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6570"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-600"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-80"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "170"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-458"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1542"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-458"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          },
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      },
      {
        "amount": {
          "value": {
            "value": "-80"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "7050"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-200"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6800"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-58"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1942"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-57"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1943"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-14"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "486"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## Neither adjustments nor promotion code nor ajustments belonging to lines
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[]}],"adjustments":[],"promotion_codes":[],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6770"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6600"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-80"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "170"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "71"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-23"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "49"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_amount": {
          "value": {
            "value": "18"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-6"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "12"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-6"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            }
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
      },
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-80"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY",
        "promotion_id": {
          "value": "DeliveryNewAmount_1"
        }
      }
    ],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "7250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": []
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": []
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": []
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": []
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "0"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": []
      }
    ],
    "promotions": [],
    "adjustments": [],
    "promotion_codes": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
## No order id
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": false
      },
      "status_details": [
        {
          "type": {
            "value": "promotion"
          },
          "status": {
            "value": "PROMOTION_SERVICE_KO"
          },
          "details": {
            "value": "Timeout has been reached because of Hystrix fallback was fired"
          }
        }
      ]
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6750"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": false
      },
      "status_details": [
        {
          "type": {
            "value": "promotion"
          },
          "status": {
            "value": "PROMOTION_SERVICE_KO"
          },
          "details": {
            "value": "Timeout has been reached because of Hystrix fallback was fired"
          }
        }
      ]
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6750"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
## No store id
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"id":{"value":"123456"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":250},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6750"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "250"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "total": {
      "value": {
        "value": "6750"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "250"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## No delivery
### Request
- DEV
```sh
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/ConfirmPurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456"},"owner_id":{"value":11111},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-503},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-65},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
### Response
- DEV
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "total": {
      "value": {
        "value": "6100"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6100"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-541"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1459"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-458"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "OrderAmountOff_1"
        },
        "description": {
          "value": "short description in Spanish para la promoción de tipo amount off"
        },
        "type": "GENERIC"
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-400"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "OrderAmountOff_1"
        }
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```
- PRE / PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "7000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "6500"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_total": {
      "value": {
        "value": "0"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "order_lines": [
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-58"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1860"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-23"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "1"
        },
        "unit": {
          "value": "3"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "173803"
        },
        "product_id": {
          "value": "2222"
        },
        "parent_id": {
          "value": "3333"
        },
        "category_id": {
          "value": "1111"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "2000"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "2000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-141"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "1859"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-60"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-24"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-57"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "1"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "unit": {
          "value": "2"
        },
        "quantity": {
          "value": "1"
        },
        "reference_id": {
          "value": "180321"
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": "500"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-39"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "461"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": "-25"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": "-14"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "MANUAL",
            "entity": "ORDER"
          }
        ]
      }
    ],
    "promotions": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-180"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": "-200"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "ORDER"
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ]
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

