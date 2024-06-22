テーブルを移行した直後気をつけること  
![image](https://github.com/yumi100/sample/assets/116421936/5fb8756a-5d12-480a-b182-f3ecf6b51beb)
![image](https://github.com/yumi100/sample/assets/116421936/3fad5e52-7457-4dbd-b67b-fe3784fd52df)
![image](https://github.com/yumi100/sample/assets/116421936/21b2d66f-c807-498a-ba44-cd73a6fb7178)
![image](https://github.com/yumi100/sample/assets/116421936/07b8de1f-89b7-4732-a7e4-f478c1baca6d)
一対多の一側に位置するフィールドは一度値を入れた後ルックアップを設定して表示を変えるのが望ましい  
![image](https://github.com/yumi100/sample/assets/116421936/526e5bdc-c695-4a3c-8ced-f7b50899d9ad)
![image](https://github.com/yumi100/sample/assets/116421936/46064a95-371c-4273-99a8-ba942235e44c)
![image](https://github.com/yumi100/sample/assets/116421936/fc2dfa05-0cd8-4434-9d3d-12c65450f0e1)
![image](https://github.com/yumi100/sample/assets/116421936/bc833f6d-53a7-4459-ab8c-11ef577571b6)  
ここまで全てウィザードを使って作っていることに注意
![image](https://github.com/yumi100/sample/assets/116421936/c517d32a-739c-4e9a-95bb-dc6d65890ff8)  
リレーションシップで繋いでいる箇所はルックアップフィールドになっている

VBA集
```vb:cmdRepCustomerList.vb
Option Compare Database

Private Sub cmdCustomerList_Click()
    DoCmd.OpenForm "CustomerList"
    
End Sub

Private Sub cmdRepCustomerList_Click()
    DoCmd.OpenReport "RepCustomerList", acViewPreview
    
End Sub
