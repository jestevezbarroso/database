# AmountEngineService. CalculatePurchaseAttempt

All requests regarding the **CalculatePurchaseAttempt** service are listed below:

- [All parameters](#all-parameters)
- [No lines](#no-lines)
- [No adjustments](#no-adjustments)
- [No promotion codes](#no-promotion-codes)
- [Neither adjustments nor promotion codes](#neither-adjustments-nor-promotion-codes)
- [Neither lines nor adjustments](#neither-lines-nor-adjustments)
- [Neither lines nor promotion codes](#neither-lines-nor-promotion-codes)
- [Neither lines nor promotion codes nor adjustments](#neither-lines-nor-promotion-codes-nor-adjustments)
- [](#)
- [](#)
- [](#)

## <a name="all-parameters"></a>All parameters 
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
  
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
  
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
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
      },
      {
        "amount": {
          "value": {
            "value": "-350"
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
- PRE
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "15820"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-4480"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "15420"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-3980"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "10026501"
        }
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
          "value": "PROMOCODE_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "10026501"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
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
- PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19800"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
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
    ],
    "promotions": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## <a name="no-lines"></a>No lines
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[],"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-950},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"},{"amount":{"value":{"value":-500},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"}],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ],
    "promotions": []
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ],
    "promotions": []
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
Excerpt from the exception happened
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
                        },
                        {
                            "methodName": "calculateCart",
                            "fileName": "ProcessManagementServiceImpl.java",
                            "lineNumber": 94,
                            "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "calculatePurchaseAttempt",
                            "fileName": "AmountEngineGrpcServer.java",
                            "lineNumber": 96,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "<generated>",
                            "lineNumber": -1,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer$$FastClassBySpringCGLIB$$2b037106",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "MethodProxy.java",
                            "lineNumber": 218,
                            "className": "org.springframework.cglib.proxy.MethodProxy",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeJoinpoint",
                            "fileName": "CglibAopProxy.java",
                            "lineNumber": 749,
                            "className": "org.springframework.aop.framework.CglibAopProxy$CglibMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "ReflectiveMethodInvocation.java",
                            "lineNumber": 163,
                            "className": "org.springframework.aop.framework.ReflectiveMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "MethodInvocationProceedingJoinPoint.java",
                            "lineNumber": 88,
                            "className": "org.springframework.aop.aspectj.MethodInvocationProceedingJoinPoint",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "annotationAround",
                            "fileName": "GrpcExceptionAspect.java",
                            "lineNumber": 72,
                            "className": "com.inditex.aqsw.framework.service.grpc.server.exceptions.aspect.GrpcExceptionAspect",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": null,
                            "lineNumber": -1,
                            "className": "sun.reflect.GeneratedMethodAccessor242",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "DelegatingMethodAccessorImpl.java",
                            "lineNumber": 43,
                            "className": "sun.reflect.DelegatingMethodAccessorImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "Method.java",
                            "lineNumber": 498,
                            "className": "java.lang.reflect.Method",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethodWithGivenArgs",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 644,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethod",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 633,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "AspectJAroundAdvice.java",
                            "lineNumber": 70,
                            "className": "org.springframework.aop.aspectj.AspectJAroundAdvice",
                            "nativeMethod": false
                        }
                        ]
                }
            }
        }
    }
}
```

## <a name="no-adjustments"></a>No adjustments
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt","payload":{"store_id":{"value":10701},"id":{"value":"123456789"},"owner_id":{"value":11111},"delivery":{"delivery_method_id":{"value":"EXPRESS"},"price":{"price":{"value":{"value":400},"currency":{"value":"EUR"}}}},"lines":[{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"GIFT_RECEIPT","price":{"price":{"value":{"value":4300},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-200},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":1},"quantity":{"value":3},"reference_id":{"value":173803},"product_id":{"value":2222},"parent_id":{"value":3333},"category_id":{"value":1111},"type":"PRODUCT","price":{"price":{"value":{"value":2000},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-180},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-70},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-800},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]},{"id":{"value":2},"quantity":{"value":2},"reference_id":{"value":180321},"type":"PRODUCT","price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}},"adjustments":[{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"LINE"},{"amount":{"value":{"value":-230},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"LINE"}]}],"adjustments":[],"promotion_codes":[{"value":"PROMOTION_CODE"}],"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}}}}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19600"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19200"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
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
            "value": "-350"
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
- PRE
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "16020"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-4280"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "15620"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-3980"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "10026501"
        }
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
            "value": "-50"
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
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "10026501"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
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
- PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "20000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19600"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
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
      }
    ],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ],
    "promotions": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## <a name="no-promotion-codes"></a>No promotion codes
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
      
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
      
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
      
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
      
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19170"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-230"
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
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
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
      },
      {
        "amount": {
          "value": {
            "value": "-230"
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
    "promotion_codes": [],
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
- PRE
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "15820"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-4480"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "15420"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-3980"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "10026501"
        }
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
    "promotion_codes": [],
    "promotions": [
      {
        "promotion_id": {
          "value": "10026501"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
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
- PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19800"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
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
    "promotion_codes": [],
    "promotions": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## <a name="no-delivery"></a>No delivery
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19000"
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
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
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
- PRE
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "15420"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-4480"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "15420"
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
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-3980"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "10026501"
        }
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
    ],
    "promotions": [
      {
        "promotion_id": {
          "value": "10026501"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
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
- PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19400"
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
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
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
    ],
    "promotions": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## <a name="neither-adjustments-nor-promotion-codes"></a>Neither adjustments nor promotion codes
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": 4300
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -200
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          },
          {
            "amount": {
              "value": {
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 1
        },
        "quantity": {
          "value": 3
        },
        "reference_id": {
          "value": 173803
        },
        "product_id": {
          "value": 2222
        },
        "parent_id": {
          "value": 3333
        },
        "category_id": {
          "value": 1111
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 2000
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -180
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
                "value": -70
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
                "value": -800
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      },
      {
        "id": {
          "value": 2
        },
        "quantity": {
          "value": 2
        },
        "reference_id": {
          "value": 180321
        },
        "type": "PRODUCT",
        "price": {
          "price": {
            "value": {
              "value": 500
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "adjustments": [
          {
            "amount": {
              "value": {
                "value": -50
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
                "value": -230
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "LINE"
          }
        ]
      }
    ],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "19370"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19200"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_adjustment": {
      "value": {
        "value": "-230"
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
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
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
            "value": "-230"
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
    "promotion_codes": [],
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
- PRE
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "16020"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_adjustment": {
      "value": {
        "value": "-4280"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_total": {
      "value": {
        "value": "15620"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": "-3980"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "ORDER",
        "promotion_id": {
          "value": "10026501"
        }
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
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "MANUAL",
        "entity": "LINE"
      }
    ],
    "promotion_codes": [],
    "promotions": [
      {
        "promotion_id": {
          "value": "10026501"
        },
        "description": {
          "value": ""
        },
        "type": "GENERIC"
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
- PRE-INT / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "20000"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "item_amount": {
      "value": {
        "value": "19900"
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
        "value": "19600"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery_amount": {
      "value": {
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [
      {
        "id": {
          "value": "1"
        },
        "quantity": {
          "value": "3"
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
        "type": "GIFT_RECEIPT",
        "price": {
          "price": {
            "value": {
              "value": "4300"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "item_amount": {
          "value": {
            "value": "12900"
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
            "value": "12900"
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
        "quantity": {
          "value": "3"
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
            "value": "6000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-250"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "5750"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      },
      {
        "id": {
          "value": "2"
        },
        "quantity": {
          "value": "2"
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
            "value": "1000"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "item_total": {
          "value": {
            "value": "950"
          },
          "currency": {
            "value": "EUR"
          }
        },
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
          }
        ]
      }
    ],
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
      }
    ],
    "promotion_codes": [],
    "promotions": []
  },
  "status": {
    "code": "OK",
    "description": null,
    "cause": null,
    "ok": true
  }
}
```

## <a name="neither-lines-nor-adjustments"></a>Neither lines nor adjustments
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-INT
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-LT
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "value": "PROMOTION_CODE"
      }
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ],
    "promotions": []
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
      {
        "code": {
          "value": "PROMOTION_CODE"
        },
        "status": "NOT_APPLIED"
      }
    ],
    "promotions": []
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
Excerpt from the exception happened
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
                        },
                        {
                            "methodName": "calculateCart",
                            "fileName": "ProcessManagementServiceImpl.java",
                            "lineNumber": 94,
                            "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "calculatePurchaseAttempt",
                            "fileName": "AmountEngineGrpcServer.java",
                            "lineNumber": 96,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "<generated>",
                            "lineNumber": -1,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer$$FastClassBySpringCGLIB$$2b037106",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "MethodProxy.java",
                            "lineNumber": 218,
                            "className": "org.springframework.cglib.proxy.MethodProxy",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeJoinpoint",
                            "fileName": "CglibAopProxy.java",
                            "lineNumber": 749,
                            "className": "org.springframework.aop.framework.CglibAopProxy$CglibMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "ReflectiveMethodInvocation.java",
                            "lineNumber": 163,
                            "className": "org.springframework.aop.framework.ReflectiveMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "MethodInvocationProceedingJoinPoint.java",
                            "lineNumber": 88,
                            "className": "org.springframework.aop.aspectj.MethodInvocationProceedingJoinPoint",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "annotationAround",
                            "fileName": "GrpcExceptionAspect.java",
                            "lineNumber": 72,
                            "className": "com.inditex.aqsw.framework.service.grpc.server.exceptions.aspect.GrpcExceptionAspect",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": null,
                            "lineNumber": -1,
                            "className": "sun.reflect.GeneratedMethodAccessor242",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "DelegatingMethodAccessorImpl.java",
                            "lineNumber": 43,
                            "className": "sun.reflect.DelegatingMethodAccessorImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "Method.java",
                            "lineNumber": 498,
                            "className": "java.lang.reflect.Method",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethodWithGivenArgs",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 644,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethod",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 633,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "AspectJAroundAdvice.java",
                            "lineNumber": 70,
                            "className": "org.springframework.aop.aspectj.AspectJAroundAdvice",
                            "nativeMethod": false
                        }
                        ]
                }
            }
        }
    }
}
```

## <a name="neither-lines-nor-promotion-codes"></a>Neither lines nor promotion codes
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [
      {
        "amount": {
          "value": {
            "value": -200
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -800
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "LINE"
      },
      {
        "amount": {
          "value": {
            "value": -950
          },
          "currency": {
            "value": "EUR"
          }
        },
        "type": "PROMOTION",
        "entity": "DELIVERY"
      },
      {
        "amount": {
          "value": {
            "value": -500
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
            "value": -200
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
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [],
    "promotions": []
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [],
    "promotions": []
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
Excerpt from the exception happened
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
                        },
                        {
                            "methodName": "calculateCart",
                            "fileName": "ProcessManagementServiceImpl.java",
                            "lineNumber": 94,
                            "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "calculatePurchaseAttempt",
                            "fileName": "AmountEngineGrpcServer.java",
                            "lineNumber": 96,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "<generated>",
                            "lineNumber": -1,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer$$FastClassBySpringCGLIB$$2b037106",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "MethodProxy.java",
                            "lineNumber": 218,
                            "className": "org.springframework.cglib.proxy.MethodProxy",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeJoinpoint",
                            "fileName": "CglibAopProxy.java",
                            "lineNumber": 749,
                            "className": "org.springframework.aop.framework.CglibAopProxy$CglibMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "ReflectiveMethodInvocation.java",
                            "lineNumber": 163,
                            "className": "org.springframework.aop.framework.ReflectiveMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "MethodInvocationProceedingJoinPoint.java",
                            "lineNumber": 88,
                            "className": "org.springframework.aop.aspectj.MethodInvocationProceedingJoinPoint",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "annotationAround",
                            "fileName": "GrpcExceptionAspect.java",
                            "lineNumber": 72,
                            "className": "com.inditex.aqsw.framework.service.grpc.server.exceptions.aspect.GrpcExceptionAspect",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": null,
                            "lineNumber": -1,
                            "className": "sun.reflect.GeneratedMethodAccessor242",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "DelegatingMethodAccessorImpl.java",
                            "lineNumber": 43,
                            "className": "sun.reflect.DelegatingMethodAccessorImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "Method.java",
                            "lineNumber": 498,
                            "className": "java.lang.reflect.Method",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethodWithGivenArgs",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 644,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethod",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 633,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "AspectJAroundAdvice.java",
                            "lineNumber": 70,
                            "className": "org.springframework.aop.aspectj.AspectJAroundAdvice",
                            "nativeMethod": false
                        }
                        ]
                }
            }
        }
    }
}
```

## <a name="neither-lines-nor-promotion-codes-nor-adjustments"></a>Neither lines nor promotion codes nor adjustments
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{
  "fullMethodName": "appmicmeccameng.v1.AmountEngineService/CalculatePurchaseAttempt",
  "payload": {
    "store_id": {
      "value": 10701
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": 11111
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": 400
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [
    ],
    "device": {
      "channel": {
        "value": "CHANNEL"
      },
      "type": {
        "value": "TYPE"
      },
      "os": {
        "value": "OS"
      }
    }
  }
}'
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [],
    "promotions": []
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
    "store_id": {
      "value": "10701"
    },
    "id": {
      "value": "123456789"
    },
    "owner_id": {
      "value": "11111"
    },
    "total": {
      "value": {
        "value": "400"
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
        "value": "400"
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
        "value": "400"
      },
      "currency": {
        "value": "EUR"
      }
    },
    "delivery": {
      "delivery_method_id": {
        "value": "EXPRESS"
      },
      "price": {
        "price": {
          "value": {
            "value": "400"
          },
          "currency": {
            "value": "EUR"
          }
        }
      }
    },
    "lines": [],
    "adjustments": [],
    "promotion_codes": [],
    "promotions": []
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
Excerpt from the exception happened
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
                        },
                        {
                            "methodName": "calculateCart",
                            "fileName": "ProcessManagementServiceImpl.java",
                            "lineNumber": 94,
                            "className": "com.inditex.mecc.appmicmeccameng.model.process.manager.ProcessManagementServiceImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "calculatePurchaseAttempt",
                            "fileName": "AmountEngineGrpcServer.java",
                            "lineNumber": 96,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "<generated>",
                            "lineNumber": -1,
                            "className": "com.inditex.mecc.appmicmeccameng.ws.server.AmountEngineGrpcServer$$FastClassBySpringCGLIB$$2b037106",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "MethodProxy.java",
                            "lineNumber": 218,
                            "className": "org.springframework.cglib.proxy.MethodProxy",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeJoinpoint",
                            "fileName": "CglibAopProxy.java",
                            "lineNumber": 749,
                            "className": "org.springframework.aop.framework.CglibAopProxy$CglibMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "ReflectiveMethodInvocation.java",
                            "lineNumber": 163,
                            "className": "org.springframework.aop.framework.ReflectiveMethodInvocation",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "proceed",
                            "fileName": "MethodInvocationProceedingJoinPoint.java",
                            "lineNumber": 88,
                            "className": "org.springframework.aop.aspectj.MethodInvocationProceedingJoinPoint",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "annotationAround",
                            "fileName": "GrpcExceptionAspect.java",
                            "lineNumber": 72,
                            "className": "com.inditex.aqsw.framework.service.grpc.server.exceptions.aspect.GrpcExceptionAspect",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": null,
                            "lineNumber": -1,
                            "className": "sun.reflect.GeneratedMethodAccessor242",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "DelegatingMethodAccessorImpl.java",
                            "lineNumber": 43,
                            "className": "sun.reflect.DelegatingMethodAccessorImpl",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "Method.java",
                            "lineNumber": 498,
                            "className": "java.lang.reflect.Method",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethodWithGivenArgs",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 644,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invokeAdviceMethod",
                            "fileName": "AbstractAspectJAdvice.java",
                            "lineNumber": 633,
                            "className": "org.springframework.aop.aspectj.AbstractAspectJAdvice",
                            "nativeMethod": false
                        },
                        {
                            "methodName": "invoke",
                            "fileName": "AspectJAroundAdvice.java",
                            "lineNumber": 70,
                            "className": "org.springframework.aop.aspectj.AspectJAroundAdvice",
                            "nativeMethod": false
                        }
                        ]
                }
            }
        }
    }
}
```

## <a name=""></a>
### Request
- DEV
```sh	
$ 
```
- PRE
```sh	
$ 
```
- PRE-INT
```sh	
$ 
```
- PRE-LT
```sh	
$ 
```

### Response
- DEV
```json

```
- PRE / PRE-INT / PRE-LT
```json

```
- PRE / PRE-INT / PRE-LT
```json

```
