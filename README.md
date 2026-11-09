
using System.ComponentModel.DataAnnotation

namespace RaceAPI.Models

    public class Participant
    {
        public int ParticipantId { get; set; }

        [Required]
        public string FirstName { get; et; } = string.Empty

        [Required]
        public string LastName { get; set; } = string.Empty;

        [Required]
        [EmailAddres
        public string Email { get; set; } = string.Empty;

        public string? PhoneNumber { get; set; }

        public ICollection<Enrolment> Enrolments { get; set; }
             new List<Enrolment>

        public ICollection<Result> Results { get; set; }
            = new List<Result>();
    

