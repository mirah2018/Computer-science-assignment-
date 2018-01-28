Module Module1

    Sub Main()

        Dim sName As String = ""
        Dim MemberIDnum As Integer = 0
        Dim sContinue As Char = "y"
        Dim NotContinue As Char = "n"


        FileOpen(1, "c:\Membershipdata\MemberRec.txt", OpenMode.Output)
        Do
            Console.WriteLine("Enter member name:")
            sName = Console.ReadLine
            Console.WriteLine("Enter member ID number:")
            MemberIDnum = Console.ReadLine

            WriteLine(1, sName)
            WriteLine(1, MemberIDnum)
            Console.WriteLine("Do you want to enter more members")
            sContinue = Console.ReadLine

        Loop Until sContinue = NotContinue



        FileClose(1)
        Console.ReadKey()



    End Sub

End Module
