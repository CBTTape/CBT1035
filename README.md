# CBT1035
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE1035 is from Hobart Spitz and contains a version of Pipes  *   FILE1035
//*           for z/OS which is written in REXX.  Documentation     *   FILE1035
//*           for the package is in PDF format, and is in member    *   FILE1035
//*           $PDFDOC, which has to be downloaded to a PC in        *   FILE1035
//*           Binary and viewed there.                              *   FILE1035
//*                                                                 *   FILE1035
//*           An introduction to zPipe is provided in the member    *   FILE1035
//*           called $EXPLAIN.                                      *   FILE1035
//*                                                                 *   FILE1035
//*           Member EXEC is a TSO XMIT of all the REXX execs, and  *   FILE1035
//*           member CEXEC is the compiled REXX members, in XMIT    *   FILE1035
//*           format.  The other individual pds members come from   *   FILE1035
//*           the EXEC member, after being RECEIVE'd.               *   FILE1035
//*                                                                 *   FILE1035
//*           email:  Hobart Spitz <orexxman@gmail.com>             *   FILE1035
//*                                                                 *   FILE1035
//*     SHORT DESCRIPTION:                                          *   FILE1035
//*                                                                 *   FILE1035
//*     zPipe - A z/OS Piping Facility that combines features of    *   FILE1035
//*     CMS/TSO Pipelines, UNIX/Linux, and REXX.  It is a free      *   FILE1035
//*     package, versus BatchPipes, which is chargeable and not     *   FILE1035
//*     in the z/OS base.                                           *   FILE1035
//*                                                                 *   FILE1035
//*     Piping originated in UNIX, where the limited budgets of     *   FILE1035
//*     academic and research organizations dictated making the     *   FILE1035
//*     best use of limited hardware.                               *   FILE1035
//*                                                                 *   FILE1035
//*     Piping is both a machine performance feature and a          *   FILE1035
//*     productivity tool.                                          *   FILE1035
//*                                                                 *   FILE1035
//*     Piping performance comes from passing the output of one     *   FILE1035
//*     program to the input of another using an in-memory          *   FILE1035
//*     buffer.  This avoids slow disk I/O and saves on hardware    *   FILE1035
//*     resources.                                                  *   FILE1035
//*                                                                 *   FILE1035
//*     Piping productivity comes from two aspects:                 *   FILE1035
//*         - It is achieved via an operator (a | b) which          *   FILE1035
//*            connects the output of a to the input of b.          *   FILE1035
//*            Compare this single character to the JCL for         *   FILE1035
//*            creating a temporary dataset in one step and         *   FILE1035
//*            passing it to another.                               *   FILE1035
//*         - Piping allows data to be passed between programs      *   FILE1035
//*            independent of the file structure.  a | b, in one    *   FILE1035
//*            context, could become a | c | d, in another.  a,     *   FILE1035
//*            b, etc. are called filters or stages.                *   FILE1035
//*                                                                 *   FILE1035
//*     zPipe delivers these features:                              *   FILE1035
//*         - It is written entirely in REXX.                       *   FILE1035
//*         - New stages can be written using simple REXX           *   FILE1035
//*            without introducing additional host commands.        *   FILE1035
//*         - It does not require additional software.              *   FILE1035
//*         - Operand syntax is that of REXX via the interpret      *   FILE1035
//*            instruction.  The user learning curve, the           *   FILE1035
//*            development costs and the execution time penalty     *   FILE1035
//*            of decoding any other operand syntax are avoided.    *   FILE1035
//*         - Processing is done at the record level, as opposed    *   FILE1035
//*            to the CPU-intensive byte level of UNIX/Linux.       *   FILE1035
//*         - Like CMS/TSO Pipelines and BatchPipes, only           *   FILE1035
//*            referenced bytes go thru the CPU.                    *   FILE1035
//*         - Also like Pipelines/BatchPipes, binary data can be    *   FILE1035
//*            processed with the same filters as text data.        *   FILE1035
//*            There are no embedded control characters or DCB      *   FILE1035
//*            parameters between stages.                           *   FILE1035
//*         - Dispatching takes place once per filter.              *   FILE1035
//*         - It free and available on the CBT Tape.                *   FILE1035
//*         - Data is passed via the REXX stack, which is           *   FILE1035
//*            managed by the zPipe module.                         *   FILE1035
//*         - The zPipe module also protects against                *   FILE1035
//*            unintentional execution of data by TSO.              *   FILE1035
//*         - A single selection filter, PICKIF, delivers the       *   FILE1035
//*            functionality of numerous Pipelines selection        *   FILE1035
//*            filters and avoids the complexity of UNIX            *   FILE1035
//*            programs such as grep and awk.  Again, operand       *   FILE1035
//*            syntax is that of REXX.                              *   FILE1035
//*         - SPEX provide reformatting, like Pipelines SPECS,      *   FILE1035
//*            again using REXX syntax.                             *   FILE1035
//*         - The CALL stage allows any REXX callable function      *   FILE1035
//*            to be invoked as filter.                             *   FILE1035
//*         - When executed as a COMMAND line, the end results      *   FILE1035
//*            are written to the terminal or primary output.       *   FILE1035
//*            making zPipe familiar to both UNIX/Linux users       *   FILE1035
//*            and intuitive to novices.                            *   FILE1035
//*         - User programs can invoke filters to manipulate        *   FILE1035
//*            REXX stack data without or without invoking the      *   FILE1035
//*            zPipe main module.  In this case, FUNCTION or        *   FILE1035
//*            SUBROUTINE invocation is used, as reported by        *   FILE1035
//*            PARSE SOURCE ... .                                   *   FILE1035
//*         - zPipe uses the familiar <, >, and >> for reading,     *   FILE1035
//*            writing and and appending data sets.  As in          *   FILE1035
//*            Pipelines, > and >> are pass-thru filters:  Data     *   FILE1035
//*            written is still available to following stages.      *   FILE1035
//*                                                                 *   FILE1035
```
