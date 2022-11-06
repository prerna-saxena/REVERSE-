# REVERSE-

int marks_summation(int* marks, int number_of_students, char gender) {
  //Write your code here.
  int i, sum = 0;
  switch (gender) 
  {
      case 'b':
        for(i = 0; i < number_of_students;++i)
        {
            sum+= *(marks + i);
            ++i;
        }
      break;
      
      case 'g':
      if (number_of_students > 1)
      {
        for(i = 1; i < number_of_students;++i)
        {
            sum+= *(marks + i);
            ++i;
        }
      }else
        {
            sum = 0;
        }
      break;
  }
  return sum;
}
