package com.example.burger2;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.View;
import android.widget.CheckBox;
import android.widget.ImageView;
import android.widget.RadioButton;
import android.widget.RadioGroup;
import android.widget.Switch;
import android.widget.Toast;
import android.widget.ToggleButton;

public class MainActivity extends AppCompatActivity {
    ToggleButton toggleButton;
    Switch aswitch;
    RadioGroup radioGroup;
    ImageView imageView2;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        aswitch = findViewById(R.id.switch1);
        toggleButton = findViewById(R.id.toggleButton);
        radioGroup = findViewById(R.id.radioGroup);
        imageView2 = findViewById(R.id.imageView2);

        radioGroup.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener() {
            @Override
            public void onCheckedChanged(RadioGroup radioGroup, int i) {
                //int id = radioGroup.getCheckedRadioButtonId();

                if (i == R.id.radioButton1) {
                    imageView2.setImageResource(R.drawable.images);
                } else if (i == R.id.radioButton2) {
                    imageView2.setImageResource(R.drawable.ps);
                } else if (i == R.id.radioButton3) {
                    imageView2.setImageResource(R.drawable.xbox);

                }

            }
        });


        // RadioButton radioButton = findViewById(id);
        //    radioButton.


        toggleButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {


            }
        });


        toggleButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {

                ((ToggleButton) view).isChecked();


            }
        });
        ;
        ;
    }

    // public void toggleClickHandler(View view){
    public void ClickHandler(View view) {

        if (view instanceof CheckBox) {
            CheckBox checkBox = ((CheckBox) view);
            if (checkBox.isChecked() && checkBox.getText().equals("PC1")) {
                imageView2.setImageResource(R.drawable.images);

            } else if (checkBox.isChecked() && checkBox.getText().equals("XBOX1")) {
                imageView2.setImageResource(R.drawable.xbox);

            }


            try {
                if (((ToggleButton) view).isChecked()) {
                    Toast.makeText(this, "on", Toast.LENGTH_SHORT).show();
                } else {
                    Toast.makeText(this, "Off", Toast.LENGTH_SHORT).show();
                }
            } catch (ClassCastException e) {
                Toast.makeText(this, "Cannot cast to toggle btn", Toast.LENGTH_SHORT).show();
            }
            try {
                if (((Switch) view).isChecked()) {
                    Toast.makeText(this, "Switch on", Toast.LENGTH_SHORT).show();
                } else {
                    Toast.makeText(this, "Switch Off", Toast.LENGTH_SHORT).show();


                }
            } catch (ClassCastException e) {
                Toast.makeText(this, "Cannot cast to toggle btn", Toast.LENGTH_SHORT).show();
            }
        }
    }
}
