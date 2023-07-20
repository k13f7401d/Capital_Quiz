using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        // A Painstakingly hand typed dictionary of all states and their capitals.
        public Dictionary<String, String> capitals = new Dictionary<string, string>
        {
            {"Alabama", "Montgomery" },
            { "Alaska", "Juneau"},
            { "Arizona", "Phoenix"},
            { "Arkansas", "Little Rock" },
            { "California", "Sacramento" },
            { "Colorado", "Sacramento" },
            { "Connecticut", "Hartford" },
            { "Delaware", "Dover" },
            { "Florida", "Tallahassee" },
            { "Georgia", "Atlanta" },
            { "Hawaii", "Honolulu" },
            { "Idaho", "Boise" },
            { "Indiana", "Indianapolis" },
            { "Iowa", "Des Moines" },
            { "Kansas", "Topeka" },
            { "Kentucky", "Frankfort" },
            { "Louisiana", "Baton Rouge" },
            { "Maine", "Augusta" },
            { "Maryland", "Annapolis" },
            { "Massachusetts", "Boston" },
            { "Michigan", "Lansing" },
            { "Minnesota","St. Paul" },
            { "Mississippi", "Jackson" },
            { "Missouri", "Jefferson City" },
            { "Montana", "Helena" },
            { "Nebraska", "Lincoln" },
            { "Nevada", "Carson City" },
            { "New Hampshire", "Concord" },
            { "New Jersey", "Trenton" },
            { "New Mexico", "Santa Fe" },
            { "New York", "Albany" },
            { "North Carolina", "Raleigh" },
            { "North Dakota", "Bismarck" },
            { "Ohio", "Columbus" },
            { "Oklahoma", "Oklahoma City" },
            { "Oregon", "Salem" },
            { "Pennsylvania", "Harrisburg" },
            { "Rhode Island", "Providence" },
            { "South Carolina", "Columbia" },
            { "South Dakota", "Pierre" },
            { "Tennessee", "Nashville" },
            { "Texas", "Austin" },
            { "Utah", "Salt Lake City" },
            { "Vermont", "Montpelier" },
            { "Virginia", "Richmond" },
            { "Washington", "Olympia" },
            { "West Virginia", "Charleston" },
            { "Wisconsin", "Madison" },
            { "Wyoming", "Cheyenne"}
        };

        // Load the List at load time
        private void Form1_Load(object sender, EventArgs e)
        {
            foreach (var element in capitals)
            {
                stateListBox.Items.Add(element.Key);
            }
        }

        private void checkButton_Click(object sender, EventArgs e)
        {
            // Here, hold this:
            var state = stateListBox.SelectedItem;
            string guess = guessTextBox.Text;
            var maybe = capitals.Values;
            int points = 0;

            // an if-else statement to check if the guess is correct.
            if (state == maybe)
            {
                MessageBox.Show("You Guessed correctly! You have " + points + " points!");
                points++;
            }
            else
            {
                MessageBox.Show("Sorry, that is incorrect. You have " + points + " points.");
                points -= 1;
            }
        }

        private void exitButton_Click(object sender, EventArgs e)
        {
            this.Close();
        }
    }
}
