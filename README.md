signature: 6e90db3191aceb620a07ff994105e33de14a0006bd2ff99c015c0b134cffbc30db6f28ba2dde09bb017e8eff5479211cf21a8dd3f97903ef6f110e24b984f506
subwallet_id: 698983191
valid_until: 1716068507
seqno: 5
op: 0
payload:
  - mode: 3
    message:
      sum_type: MessageInternal
      message_internal:
        ihr_disabled: true
        bounce: true
        bounced: false
        src: ""
        dest: 0:977be0be33a74415b0a9caffdbec244e8bdd1a11c6136742a88a1afb0e3d17e9
        value:
          grams: "98527371"
          other: {}
        ihr_fee: "0"
        fwd_fee: "0"
        created_lt: 0
        created_at: 0
        init: null
        body:
          is_right: true
          value:
            sum_type: NftTransfer
            op_code: 1607220500
            value:
              query_id: 6083770390913275000
              new_owner: 0:40b7175857c497fe9033b1caaa32516d7b1fb49e68b9ceac67170dc247a5c959
              response_destination: 0:dfbd5be8497fdc0c9fcbdfc676864840ddf8ad6423d6d5657d9b0e8270d6c8ac
              custom_payload: null
              forward_amount: "1"
              forward_payload:
                is_right: true
                value:
                  sum_type: TextComment
                  op_code: 0
                  value:
                    text: ""
