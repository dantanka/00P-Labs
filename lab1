using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace labis1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void button1_Click(object sender, EventArgs e)
        {
            double x;
            double y;
            double result;
            x = Convert.ToDouble(textBox1.Text);
            y = Convert.ToDouble(textBox2.Text);
            result = 1 * Math.Pow(x - 2, 2) + 1 * (x - 2) * Math.Sin(x - 2) + 1 * Math.Pow(Math.Sin(x - 2), 2) + 3 * Math.Pow(y - 0, 2);
            textBox3.Text = Convert.ToString(result);


        }

        private void textBox1_KeyPress(object sender, KeyPressEventArgs e)
        {
            switch (e.KeyChar)
            {
                case ',':
                case '-':
                case '0':
                case '1':
                case '2':
                case '3':
                case '4':
                case '5':
                case '6':
                case '7':
                case '8':
                case '9':
                    break;
                case '\b':
                    break;
                default:
                    e.KeyChar = (char)0;
                    break;
                case '\r':
                    if (string.IsNullOrEmpty(textBox1.Text))
                    {
                        MessageBox.Show("TextBox cannot be empty");
                        return;
                    }
                    break;
            
            }
        }

        private void textBox2_Validating(object sender, CancelEventArgs e)
        {
            double a;
            try
            {
                a = Convert.ToDouble(textBox2.Text);
            }
            catch
            {
                MessageBox.Show("Only numbers");
                e.Cancel = true;
            }

        }
    }
}
