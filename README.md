
using System.ComponentModel.DataAnnotations;

namespace RaceAPI.Models
{
    public class Participant
    {
        public int ParticipantId { get; set; }

        [Required]
        public string FirstName { get; set; } = string.Empty;

        [Required]
        public string LastName { get; set; } = string.Empty;

        [Required]
        [EmailAddress]
        public string Email { get; set; } = string.Empty;

        public string? PhoneNumber { get; set; }

        public ICollection<Enrolment> Enrolments { get; set; }
            = new List<Enrolment>();

        public ICollection<Result> Results { get; set; }
            = new List<Result>();
    }

