# СompanyCoreLib2

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CompanyCoreLIB
{
    public class Analytics
    {
        public List<DateTime> PopularMonths(List<DateTime> dates)
        {
            var DateTimeWithCounterList = new List<DateTimeWithCounter>();

            int PreviousYear = DateTime.Now.Year - 1;
            foreach (DateTime IterDate in dates)
            {
                if (IterDate.Year == PreviousYear)
                {
                    var DateMonthStart = new DateTime(date.Year, date.Month, 1, 0, 0, 0);

                    var index = DateTimeWithCounterList.FindIndex(item => item.DateTimeProp == DateMonthStart);

                    if (index == -1)
                    {
                        DateTimeWithCounterList.
                            Add(new DateTimeWithCounter(DateMonthStart));
                    }
                    else
                    {
                        DateTimeWithCounterList[index].Counter++;
                    }
                }
            }
            ...
    }
    }
