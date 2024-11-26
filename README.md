1.File Read & Write Challenge 🖋️: Create a program that reads a file and writes a modified version to a new file.


       input_file = 'input.txt'   
       output_file = 'output.txt'
   
         content = infile.read()
        

         modified_content = content.upper()
        
         outfile.write(modified_content)
        
       print(f"Modified content written to '{output_file}' successfully!")

       except FileNotFoundError:
             print(f"The file '{input_file}' does not exist. Please check the file name.")
        except Exception as e:
             print(f"An error occurred: {e}")


2.Error Handling Lab 🧪: Ask the user for a filename and handle errors if it doesn’t exist or can’t be read.

             filename = input("Please enter the filename: ")

            with open(filename, 'r') as file:
        
            content = file.read()
            print("File content:")
            print(content)

         except FileNotFoundError:
                print(f"Error: The file '{filename}' does not exist.")
         except PermissionError:
                print(f"Error: You do not have permission to read the file '{filename}'.")
         except Exception as e:
                print(f"An unexpected error occurred: {e}")
