# AplicacionesPrimerParcial-ChangoluisaEdwin
Codigo de MainActivity,java
package com.example.sumade2numeros;

import androidx.appcompat.app.AppCompatActivity;

import android.annotation.SuppressLint;
import android.os.Bundle;
import android.preference.EditTextPreference;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;


public class MainActivity extends AppCompatActivity implements View.OnClickListener{
   EditText et1, et2;
   TextView tv1;
   Button btnSumar;

    @SuppressLint("MissingInflatedId")
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        et1=(EditText)findViewById(R.id.txtNumero1);
        et2=(EditText)findViewById(R.id.txtNumero2);
        tv1=(TextView)findViewById(R.id.lblResultado);
        btnSumar=(Button)findViewById(R.id.btnSumar);
        btnSumar.setOnClickListener(this);
    }

    @Override
    public void onClick(View v) {
        float n1, n2, res;
        n1=Float.parseFloat(et1.getText().toString());
        n2=Float.parseFloat(et2.getText().toString());
        res=n1+n2;
        tv1.setText("El Resultado es: "+res);
        Toast.makeText(getApplicationContext(), "El resultado es: "+res, Toast.LENGTH_LONG).show();
    }
}
![SUMAAAA](https://github.com/EdwinGuamani/AplicacionesPrimerParcial-ChangoluisaEdwin/assets/133244382/ce7c0d58-aefa-48a8-88e6-bf5da8d5a1e3)
![555555555555](https://github.com/EdwinGuamani/AplicacionesPrimerParcial-ChangoluisaEdwin/assets/133244382/30ee07a8-a2fe-41d6-b3a5-14073393242c)
