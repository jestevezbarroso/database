# AmountEngineService. CalculateDeliveryPromotion

All requests regarding the **CalculateDeliveryPromotion** service are listed below:

- [All parameters](#all-parameters)
- [No any adjustments](#no-any-adjustments)
- [Neither any adjustments nor promotion codes](#neither-any-adjustments-nor-promotion-codes)
- [No promotion codes](#no-promotion-codes)
- [No delivery options](#no-delivery-options)
- [No delivery options (Standard)](#no-delivery-options-standard)
- [No delivery options (Express)](#no-delivery-options-express)
- [Neither delivery options nor any adjustments](#neither-delivery-options-nor-any-adjustments)
- [Neither delivery options (Express) nor adjustments (Manual-delivery)](#neither-delivery-options-express-nor-adjustments-manual-delivery)
- [Neither delivery options (Standard) nor adjustments (Manual-delivery)](#neither-delivery-options-standard-nor-adjustments-manual-delivery)
- [No adjustments (Manual-delivery)](#no-adjustments-manual-delivery)
- [Neither delivery options nor adjustments (Manual-delivery)](#neither-delivery-options-nor-adjustments-manual-delivery)
- [Neither promotion codes nor delivery options](#neither-promotion-codes-nor-delivery-options)
- [Neither promotion codes nor delivery options nor adjustments](#neither-promotion-codes-nor-delivery-options-nor-adjustments)
- [Neither promotion codes nor adjustments (Manual-delivery)](#neither-promotion-codes-nor-adjustments-manual-delivery)


## All parameters
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
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
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "120"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-20"
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-380"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "120"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-330"
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
- PRE / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "450"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": []
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
- PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-500"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-500"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            }
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
              "value": "11041501"
            }
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            },
            "description": {
              "value": "Estandar Cross"
            },
            "type": "GENERIC"
          },
          {
            "promotion_id": {
              "value": "11041501"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
## No any adjustments
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[{"value":"PROMOCODE_CODE"}],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
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
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-20"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-20"
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
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-330"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-330"
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
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
- PRE / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
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
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
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
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [],
        "delivery_promotions": []
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
- PRE-INT
```
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
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
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-500"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-500"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            }
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
              "value": "11041501"
            }
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            },
            "description": {
              "value": "Estandar Cross"
            },
            "type": "GENERIC"
          },
          {
            "promotion_id": {
              "value": "11041501"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
## Neither any adjustments nor promotion codes
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
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
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-20"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-20"
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
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-330"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-330"
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
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
- PRE / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
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
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
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
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [],
        "delivery_promotions": []
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
- PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
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
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-500"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-500"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            }
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
              "value": "11041501"
            }
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            },
            "description": {
              "value": "Estandar Cross"
            },
            "type": "GENERIC"
          },
          {
            "promotion_id": {
              "value": "11041501"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
## No promotion codes
### Request
- DEV
```sh	
$ curl -X POST \
  http://develop-mecfamemic.axdesocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE
```sh	
$ curl -X POST \
  https://pre-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-INT
```sh	
$ curl -X POST \
  https://preint-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
```
- PRE-LT
```sh	
$ curl -X POST \
  https://prelt-mecfamemic-purchase-private.za.axpreecocp1.central.inditex.grp/amiga/grpc-invoker \
  -H 'Content-Type: application/json' \
  -d '{"fullMethodName":"appmicmeccameng.v1.AmountEngineService/CalculateDeliveryPromotions","payload":{"store_id":{"value":10701},"owner_id":{"value":2222222},"device":{"channel":{"value":"CHANNEL"},"type":{"value":"TYPE"},"os":{"value":"OS"}},"base_amount":{"value":{"value":7000},"currency":{"value":"EUR"}},"adjustments":[{"amount":{"value":{"value":-30},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"ORDER"},{"amount":{"value":{"value":-50},"currency":{"value":"EUR"}},"type":"MANUAL","entity":"DELIVERY"},{"amount":{"value":{"value":-100},"currency":{"value":"EUR"}},"type":"PROMOTION","entity":"DELIVERY"}],"promotion_codes":[],"delivery_options":[{"delivery_method_id":{"value":"Express"},"price":{"price":{"value":{"value":190},"currency":{"value":"EUR"}}}},{"delivery_method_id":{"value":"Standard"},"price":{"price":{"value":{"value":500},"currency":{"value":"EUR"}}}}]}}'
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
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-70"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "120"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-20"
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-380"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "120"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-330"
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DeliveryNewAmount_1"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
- PRE / PRE-LT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "450"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": []
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
- PRE-INT
```json
{
  "payload": {
    "calculation_status": {
      "global_status": {
        "value": true
      },
      "status_details": []
    },
    "calculated_delivery_promotions": [
      {
        "delivery_method_id": {
          "value": "Express"
        },
        "price": {
          "price": {
            "value": {
              "value": "190"
            },
            "currency": {
              "value": "EUR"
            }
          }
        },
        "delivery_amount": {
          "value": {
            "value": "190"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-50"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_total": {
          "value": {
            "value": "140"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustments": [
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
            "entity": "DELIVERY"
          }
        ],
        "delivery_promotions": []
      },
      {
        "delivery_method_id": {
          "value": "Standard"
        },
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
        "delivery_amount": {
          "value": {
            "value": "500"
          },
          "currency": {
            "value": "EUR"
          }
        },
        "delivery_adjustment": {
          "value": {
            "value": "-500"
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
        "delivery_adjustments": [
          {
            "amount": {
              "value": {
                "value": "-500"
              },
              "currency": {
                "value": "EUR"
              }
            },
            "type": "PROMOTION",
            "entity": "DELIVERY",
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            }
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
              "value": "11041501"
            }
          }
        ],
        "delivery_promotions": [
          {
            "promotion_id": {
              "value": "DPRange##12109##STANDARD"
            },
            "description": {
              "value": "Estandar Cross"
            },
            "type": "GENERIC"
          },
          {
            "promotion_id": {
              "value": "11041501"
            },
            "description": {
              "value": ""
            },
            "type": "GENERIC"
          }
        ]
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
## No delivery options
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
## No delivery options (Standard)
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
## No delivery options (Express)
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
## Neither delivery options nor any adjustments
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
## Neither delivery options (Express) nor adjustments (Manual-delivery)
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
## Neither delivery options (Standard) nor adjustments (Manual-delivery)
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
## No adjustments (Manual-delivery)
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
## Neither delivery options nor adjustments (Manual-delivery)
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
## Neither promotion codes nor delivery options
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
## Neither promotion codes nor delivery options nor adjustments
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
## Neither promotion codes nor adjustments (Manual-delivery)
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
