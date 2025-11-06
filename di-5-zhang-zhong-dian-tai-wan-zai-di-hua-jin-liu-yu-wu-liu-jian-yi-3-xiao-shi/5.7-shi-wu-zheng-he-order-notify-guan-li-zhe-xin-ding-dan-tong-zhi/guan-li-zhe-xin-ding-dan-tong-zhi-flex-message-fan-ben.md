# 管理者新訂單通知 (Flex Message 範本)

```json
{
  "type": "bubble",
  "header": {
    "type": "box",
    "layout": "horizontal",
    "contents": [
      {
        "type": "text",
        "text": "新訂單通知",
        "weight": "bold",
        "color": "#ffffff",
        "size": "sm"
      }
    ],
    "backgroundColor": "#c54431",
    "paddingTop": "19px",
    "paddingAll": "12px",
    "paddingBottom": "16px"
  },
  "body": {
    "type": "box",
    "layout": "vertical",
    "contents": [
      {
        "type": "text",
        "text": "來自 {{customer_last_name}}{{customer_first_name}} 的訂單",
        "weight": "bold",
        "size": "xl",
        "margin": "md",
        "color": "#1f2d3d"
      },
      {
        "type": "box",
        "layout": "vertical",
        "margin": "xxl",
        "spacing": "sm",
        "contents": [
          {
            "type": "text",
            "text": "▍訂單資訊",
            "color": "#555555",
            "size": "sm",
            "weight": "bold"
          },
          {
            "type": "box",
            "layout": "horizontal",
            "contents": [
              {
                "type": "text",
                "text": "訂單編號：",
                "size": "sm",
                "color": "#555555",
                "flex": 0
              },
              {
                "type": "text",
                "text": "#{{order_number}}",
                "size": "sm",
                "color": "#111111",
                "align": "end"
              }
            ]
          },
          {
            "type": "separator",
            "margin": "lg"
          },
          {
            "type": "text",
            "text": "▍訂購項目",
            "color": "#555555",
            "size": "sm",
            "weight": "bold",
            "margin": "lg"
          },
          {
            "type": "text",
            "text": "{{order_items_nums}}",
            "size": "sm",
            "color": "#111111",
            "wrap": true
          },
          {
            "type": "separator",
            "margin": "lg"
          },
          {
            "type": "text",
            "text": "▍訂單金額",
            "color": "#555555",
            "size": "sm",
            "weight": "bold",
            "margin": "lg"
          },
          {
            "type": "box",
            "layout": "horizontal",
            "contents": [
              {
                "type": "text",
                "text": "總金額：",
                "size": "sm",
                "color": "#555555",
                "flex": 0
              },
              {
                "type": "text",
                "text": "{{order_total}}",
                "size": "sm",
                "color": "#111111",
                "align": "end"
              }
            ]
          },
          {
            "type": "separator",
            "margin": "lg"
          },
          {
            "type": "text",
            "text": "▍金物流資訊",
            "color": "#555555",
            "size": "sm",
            "weight": "bold",
            "margin": "lg"
          },
          {
            "type": "box",
            "layout": "horizontal",
            "margin": "md",
            "contents": [
              {
                "type": "text",
                "text": "金流類型：",
                "size": "sm",
                "color": "#555555",
                "flex": 0
              },
              {
                "type": "text",
                "text": "{{order_payment_method}}",
                "size": "sm",
                "color": "#111111",
                "align": "end",
                "wrap": true
              }
            ]
          },
          {
            "type": "box",
            "layout": "horizontal",
            "contents": [
              {
                "type": "text",
                "text": "物流類型：",
                "size": "sm",
                "color": "#555555",
                "flex": 0
              },
              {
                "type": "text",
                "text": "{{order_shipping_method}}",
                "size": "sm",
                "color": "#111111",
                "align": "end",
                "wrap": true
              }
            ]
          },
          {
            "type": "separator",
            "margin": "lg"
          },
          {
            "type": "text",
            "text": "▍訂單備註",
            "color": "#555555",
            "size": "sm",
            "weight": "bold",
            "margin": "lg"
          },
          {
            "type": "text",
            "text": "{{order_customer_note}}",
            "size": "sm",
            "color": "#111111",
            "wrap": true
          },
          {
            "type": "box",
            "layout": "vertical",
            "contents": []
          }
        ]
      }
    ],
    "paddingAll": "20px",
    "backgroundColor": "#fdf6ec"
  },
  "footer": {
    "type": "box",
    "layout": "vertical",
    "spacing": "sm",
    "contents": [
      {
        "type": "button",
        "style": "primary",
        "height": "sm",
        "action": {
          "type": "uri",
          "label": "在後台查看該筆訂單",
          "uri": "{{order_admin_url}}"
        },
        "color": "#000000"
      },
      {
        "type": "text",
        "text": "點擊上方按鈕追蹤訂單",
        "color": "#FFFFFF",
        "size": "xxs",
        "align": "center"
      }
    ],
    "flex": 0,
    "backgroundColor": "#c54431"
  },
  "styles": {
    "body": {
      "backgroundColor": "#fdf6ec"
    }
  }
}
```
