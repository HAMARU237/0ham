using System;
using System.Runtime.InteropServices.Marshalling;

namespace WinFormsApp1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void label2_Click(object sender, EventArgs e)
        {

        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void button1_Click(object sender, EventArgs e)
        {
            string inputNUM1 = NUM1.Text;
            string inputNUM2 = NUM2.Text;
            int iNUM1 = Int32.Parse(inputNUM1);
            int iNUM2 = Int32.Parse(inputNUM2);
            int iResult = iNUM1 + iNUM2;
            result.Text = iResult.ToString();
        }

        private void resukt_MaskInputRejected(object sender, MaskInputRejectedEventArgs e)
        {

        }

        private void button2_Click(object sender, EventArgs e)
        {
            string inputNUM1 = NUM1.Text;
            string inputNUM2 = NUM2.Text;
            int iNUM1 = Int32.Parse(inputNUM1);
            int iNUM2 = Int32.Parse(inputNUM2);
            int iResult = iNUM1 - iNUM2;
            result.Text = iResult.ToString();
        }

        private void button4_Click(object sender, EventArgs e)
        {
            string inputNUM1 = NUM1.Text;
            string inputNUM2 = NUM2.Text;
            int iNUM1 = Int32.Parse(inputNUM1);
            int iNUM2 = Int32.Parse(inputNUM2);
            int iResult = iNUM1 * iNUM2;
            result.Text = iResult.ToString();
        }

        private void button5_Click(object sender, EventArgs e)
        {
            string inputNUM1 = NUM1.Text;
            string inputNUM2 = NUM2.Text;
            int iNUM1 = Int32.Parse(inputNUM1);
            int iNUM2 = Int32.Parse(inputNUM2);
            int iResult = iNUM1 / iNUM2;
            result.Text = iResult.ToString();
        }

        private void button3_Click(object sender, EventArgs e)
        {
            NUM1.Text = "";
            NUM2.Text = "";
            result.Text = "";
        }
    }
}
