# FileCheckInWindowForms
You can check file exist or not in window forms

////////////////////////////////********************************************//////////////////////////////////////

string filePath = new DirectoryInfo(Environment.CurrentDirectory).Parent.Parent.FullName;  // This is Root Directory

            var fullPath = Path.Combine(filePath, @"License");           // Here full path till your folder
            DirectoryInfo dinfo = new DirectoryInfo(fullPath);           // Get all information of full path
            FileInfo[] smFiles = dinfo.GetFiles("tt.txt");                // Get All files in folder
