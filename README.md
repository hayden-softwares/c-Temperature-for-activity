# c-Temperature-for-activity
text that you can copy-paste in visual studio to impress your friends
            
            
            
            
            
            
            while (true)
            {
                int Temperature = 0;
                string errorMessage = "This is not a string try again";
                var stringTemp = String.Empty;
                bool ValidParse = false;
                bool activate = true;
                bool ifcatched = false;






                Console.WriteLine("Enter the current temperature ");
                stringTemp = Console.ReadLine();
                
                
                    ValidParse = int.TryParse(stringTemp, out Temperature);
                


                if (ValidParse == true)
                {    try
                    {
                        int.Parse(stringTemp, (System.Globalization.NumberStyles)Temperature);
                    } catch { ifcatched = true; ValidParse = true; }
                    if (ifcatched == true)
                    {
                        Convert.ToDecimal(Temperature);
                    }


                }
                else
                {
                    Console.WriteLine(errorMessage);
                    activate = false;


                }
                if (activate == true)
                    if (Temperature <= 0)
                    {
                        Console.WriteLine("its freezing here you should put on a suit");
                    }
                    else if (Temperature < 15)
                    {
                        Console.WriteLine("its cold here you should put on a coat");
                    }
                    else if (Temperature > 20)
                    {
                        Console.WriteLine("a great day");
                    } else if (Temperature < 20)
                    {
                        Console.WriteLine("its cold here you should put on a coat");
                    }
            }
