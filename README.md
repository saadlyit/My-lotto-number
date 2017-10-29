using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows;
using System.Windows.Controls;
using System.Windows.Data;
using System.Windows.Documents;
using System.Windows.Input;
using System.Windows.Media;
using System.Windows.Media.Imaging;
using System.Windows.Navigation;
using System.Windows.Shapes;

namespace Lotto_Number
{
    /// <summary>
    /// Interaction logic for MainWindow.xaml
    /// </summary>
    public partial class MainWindow : Window
    {
        public MainWindow()
        {
            InitializeComponent();
        }

        private void button_Click(object sender, RoutedEventArgs e)
        {
            
            Random rndnumbers = new Random();
            int[] num = new int[6];
            


            for (int i = 1; i <= 6; i++)

            {

                int variable;
                variable = rndnumbers.Next(1, 52);
                
                if (i == 1)
                {
                    textBox.Text = variable.ToString();
                    num[0] = int.Parse(textBox.Text);
                    
                }
                if (i == 2)
                {
                    textBox1.Text = variable.ToString();
                    num[1] = int.Parse(textBox1.Text);
                    
                }
                if (i == 3)
                {
                    textBox2.Text = variable.ToString();
                    num[2] = int.Parse(textBox2.Text);                    
                    
                }
                
                if (i == 4)
                {
                    textBox3.Text = variable.ToString();
                    num[3] = int.Parse(textBox3.Text);
                   
                }
                if (i == 5)
                {
                    textBox4.Text = variable.ToString();
                    num[4] = int.Parse(textBox4.Text);
                                    }
                if (i == 6)
                {
                    textBox5.Text = variable.ToString();
                    num[5] = int.Parse(textBox5.Text);
                    
                }
                //VAR is useful when you're not sure what type of value or values will be returned
                            
            }
            

        }

        private void textBox1_TextChanged(object sender, TextChangedEventArgs e)
        {

        }

        private void button1_Click(object sender, RoutedEventArgs e)
        {
            Random rndnumbers = new Random();
            int[] num = new int[6];



            for (int i = 1; i <= 6; i++)

            {

                int variable;
                variable = rndnumbers.Next(1, 59);

                if (i == 1)
                {
                    textBox.Text = variable.ToString();
                    num[0] = int.Parse(textBox.Text);

                }
                if (i == 2)
                {
                    textBox1.Text = variable.ToString();
                    num[1] = int.Parse(textBox1.Text);

                }
                if (i == 3)
                {
                    textBox2.Text = variable.ToString();
                    num[2] = int.Parse(textBox2.Text);

                }

                if (i == 4)
                {
                    textBox3.Text = variable.ToString();
                    num[3] = int.Parse(textBox3.Text);

                }
                if (i == 5)
                {
                    textBox4.Text = variable.ToString();
                    num[4] = int.Parse(textBox4.Text);
                }
                if (i == 6)
                {
                    textBox5.Text = variable.ToString();
                    num[5] = int.Parse(textBox5.Text);

                }
                //VAR is useful when you're not sure what type of value or values will be returned

            }
        }
    }
}
