# kamathebullet
ing System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApplication4
{
    public partial class Form1 : Form
    {
        public Form1()
        {

InitializeComponent();
            pictureBox1.Image = Image.FromFile(@"D:\kursach\1HmcPp7i0kg.png");
            pictureBox2.Visible = false;
            pictureBox3.Visible = false;

        }

        private void button1_Click(object sender, EventArgs e)
        {

            label1.Visible = true;
            checkBox1.Enabled = false;
            button2.Enabled = true;
            button3.Enabled = true;
            button1.Enabled = false;
            pictureBox2.Visible = true;
            pictureBox3.Visible = true;
            pictureBox1.Image = Image.FromFile(@"D:\kursach\стол.png");
            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

            if (checkBox1.Checked == true)
            {
                label2.Text = "Игра с компьютером";
               // int summ = Convert.ToInt32(label5.Text);   Перевод из строки в число
               // string str = Convert.ToString(summ);       Перевод из числа в строку
}
else
            {
label2.Text = "Игра с человеком";
}
        }

        private void button2_Click(object sender, EventArgs e)
        {
            checkBox1.Enabled = true;
            button1.Enabled = true;
            button2.Enabled = false;
            button3.Enabled = false;
            label1.Visible = false;
            label1.Text = "Ход игрока №1";
            label3.Text = "0";
            label4.Text = "0";
            label5.Text = "0";
            pictureBox1.Image = Image.FromFile(@"D:\kursach\1HmcPp7i0kg.png");
            pictureBox2.Visible = false;
            pictureBox3.Visible = false;

        }

        private void button3_Click(object sender, EventArgs e)
        {

            Random random = new Random();
            int a, b, summ1, summ, qwerty, a1, b1;
            int max = Convert.ToInt32(label6.Text);
            int hod = Convert.ToInt32(label5.Text);

            if (checkBox1.Checked == false)
            {
                if (hod == max)
                {

                    button3.Enabled = false;
                }

                if (hod < max)
                {
                    hod = hod + 1;
                    string str1 = Convert.ToString(hod);
                    label5.Text = str1;

                    switch (label1.Text)
                    {
                        case ("Ход игрока №1"):
                            {
                                label1.Text = "Ход игрока №2";
                                a = random.Next(1, 6);
                                b = random.Next(1, 6);
                                if ((a == 1) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 1) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 1) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 1) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 1) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 1) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 2) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 2) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 2) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 2) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 2) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 2) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 3) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 3) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 3) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 3) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 3) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 3) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 4) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 4) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 4) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 4) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 4) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 4) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 5) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 5) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 5) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 5) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 5) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 5) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 6) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 6) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 6) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 6) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 6) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 6) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label3.Text);
                                    summ1 = a + b;
                                    summ1 = summ1 + lab;
                                    string str = Convert.ToString(summ1);
                                    label3.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                label1.Text = "Ход игрока №2";
                                break;
                            }
                        case ("Ход игрока №2"):
                            {
                                label1.Text = "Ход игрока №1";
                                a = random.Next(1, 6);
                                b = random.Next(1, 6);
                                if ((a == 1) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 1) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 1) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 1) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 1) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 1) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 2) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 2) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 2) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 2) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 2) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 2) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 3) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 3) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 3) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 3) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 3) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 3) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 4) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 4) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 4) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 4) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 4) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 4) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 5) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 5) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 5) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 5) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 5) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 5) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                if ((a == 6) && (b == 1))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");
                                    break;
                                }
                                if ((a == 6) && (b == 2))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                                    break;
                                }
                                if ((a == 6) && (b == 3))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");
                                    break;
                                }
                                if ((a == 6) && (b == 4))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");
                                    break;
                                }
                                if ((a == 6) && (b == 5))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");
                                    break;
                                }
                                if ((a == 6) && (b == 6))
                                {
                                    int lab = Convert.ToInt32(label4.Text);
                                    summ = a + b;
                                    summ = summ + lab;
                                    string str = Convert.ToString(summ);
                                    label4.Text = str;
                                    pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                                    pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");
                                    break;
                                }
                                label1.Text = "Ход игрока №1";
                                break;
                            }
                    }

                }
                else
                {
                    if (hod == max)
                    {

                        button3.Enabled = false;
                    }

                    if (hod < max)
                    {
                        hod = hod + 1;
                        string str2 = Convert.ToString(hod);
                        label5.Text = str2;

                        label2.Visible = true;
                        label1.Text = "Игра с компьютером";
a = random.Next(1, 6);
                        b = random.Next(1, 6);
                        if ((a == 1) && (b == 1))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                        }
                        if ((a == 1) && (b == 2))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                        }
                        if ((a == 1) && (b == 3))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                        }
                        if ((a == 1) && (b == 4))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                        }
                        if ((a == 1) && (b == 5))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                        }
                        if ((a == 1) && (b == 6))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                        }
                        if ((a == 2) && (b == 1))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                        }
                        if ((a == 2) && (b == 2))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                        }
                        if ((a == 2) && (b == 3))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                        }
                        if ((a == 2) && (b == 4))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                        }
                        if ((a == 2) && (b == 5))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                        }
                        if ((a == 2) && (b == 6))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                        }
                        if ((a == 3) && (b == 1))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                        }
                        if ((a == 3) && (b == 2))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                        }
                        if ((a == 3) && (b == 3))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                        }
                        if ((a == 3) && (b == 4))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                        }
                        if ((a == 3) && (b == 5))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                        }
                        if ((a == 3) && (b == 6))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                        }
                        if ((a == 4) && (b == 1))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                        }
                        if ((a == 4) && (b == 2))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                        }
                        if ((a == 4) && (b == 3))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                        }
                        if ((a == 4) && (b == 4))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                        }
                        if ((a == 4) && (b == 5))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                        }
                        if ((a == 4) && (b == 6))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                        }
                        if ((a == 5) && (b == 1))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                        }
                        if ((a == 5) && (b == 2))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                        }
                        if ((a == 5) && (b == 3))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                        }
                        if ((a == 5) && (b == 4))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                        }
                        if ((a == 5) && (b == 5))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                        }
                        if ((a == 5) && (b == 6))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                        }
                        if ((a == 6) && (b == 1))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                        }
                        if ((a == 6) && (b == 2))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                        }
                        if ((a == 6) && (b == 3))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                        }
                        if ((a == 6) && (b == 4))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                        }
                        if ((a == 6) && (b == 5))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                        }
                        if ((a == 6) && (b == 6))
                        {
                            int lab = Convert.ToInt32(label3.Text);
                            summ1 = a + b;
                            summ1 = summ1 + lab;
                            string str = Convert.ToString(summ1);
                            label3.Text = str;
                            pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                            pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                        }
                        a1 = random.Next(1, 6);
                        b1 = random.Next(1, 6);
                        int qw = Convert.ToInt32(label4.Text);
                        qwerty = a1 + b1;
                        qwerty = qwerty + qw;
                        string str1 = Convert.ToString(qwerty);
                        label4.Text = str1;
                    }
                }
            }
            else
            {

                if (hod == max)
                {

                    button3.Enabled = false;
                }

                if (hod < max)
                {
                    hod = hod + 1;
                    string str2 = Convert.ToString(hod);
                    label5.Text = str2;

                    label2.Visible = true;
                    label1.Text = "Игра с компьютером";
a = random.Next(1, 6);
                    b = random.Next(1, 6);
                    if ((a == 1) && (b == 1))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                    }
                    if ((a == 1) && (b == 2))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");
                    }
                    if ((a == 1) && (b == 3))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                    }
                    if ((a == 1) && (b == 4))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                    }
                    if ((a == 1) && (b == 5))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                    }
                    if ((a == 1) && (b == 6))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\1.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                    }
                    if ((a == 2) && (b == 1))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                    }
                    if ((a == 2) && (b == 2))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                    }
                    if ((a == 2) && (b == 3))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                    }
                    if ((a == 2) && (b == 4))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                    }
                    if ((a == 2) && (b == 5))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                    }
                    if ((a == 2) && (b == 6))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\2.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                    }
                    if ((a == 3) && (b == 1))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                    }
                    if ((a == 3) && (b == 2))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                    }
                    if ((a == 3) && (b == 3))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                    }
                    if ((a == 3) && (b == 4))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                    }
                    if ((a == 3) && (b == 5))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                    }
                    if ((a == 3) && (b == 6))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\3.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                    }
                    if ((a == 4) && (b == 1))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                    }
                    if ((a == 4) && (b == 2))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                    }
                    if ((a == 4) && (b == 3))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                    }
                    if ((a == 4) && (b == 4))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                    }
                    if ((a == 4) && (b == 5))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                    }
                    if ((a == 4) && (b == 6))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\4.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                    }
                    if ((a == 5) && (b == 1))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                    }
                    if ((a == 5) && (b == 2))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                    }
                    if ((a == 5) && (b == 3))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                    }
                    if ((a == 5) && (b == 4))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                    }
                    if ((a == 5) && (b == 5))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                    }
                    if ((a == 5) && (b == 6))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\5.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                    }
                    if ((a == 6) && (b == 1))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\1.png");

                    }
                    if ((a == 6) && (b == 2))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\2.png");

                    }
                    if ((a == 6) && (b == 3))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\3.png");

                    }
                    if ((a == 6) && (b == 4))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\4.png");

                    }
                    if ((a == 6) && (b == 5))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\5.png");

                    }
                    if ((a == 6) && (b == 6))
                    {
                        int lab = Convert.ToInt32(label3.Text);
                        summ1 = a + b;
                        summ1 = summ1 + lab;
                        string str = Convert.ToString(summ1);
                        label3.Text = str;
                        pictureBox2.Image = Image.FromFile(@"D:\kursach\6.png");
                        pictureBox3.Image = Image.FromFile(@"D:\kursach\6.png");

                    }
                    a1 = random.Next(1, 6);
                    b1 = random.Next(1, 6);
                    int qw = Convert.ToInt32(label4.Text);
                    qwerty = a1 + b1;
                    qwerty = qwerty + qw;
                    string str1 = Convert.ToString(qwerty);
                    label4.Text = str1;

                }

            }
        }    




        private void button4_Click(object sender, EventArgs e)
        {
            MessageBox.Show(label1.Text, "Таблица рекордов", MessageBoxButtons.OK, MessageBoxIcon.Information);
        }

        private void button5_Click(object sender, EventArgs e)
        {
Close();
        }

        private void Form1_Load(object sender, EventArgs e)
        {
            label1.Visible = false;
            label2.Visible = false;
            button2.Enabled = false;
            button3.Enabled = false;
        }

        private void pictureBox2_Click(object sender, EventArgs e)
        {

        }
    }
}

